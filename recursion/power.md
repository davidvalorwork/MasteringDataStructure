# Power Function using Recursion

If I said Pow(2,3) is 2 * 2 * 2

## C++

Time complexity: O(n)

int pow(int m, int n)
{
  if(n==0)
    return 1;
  return pow(m,n-1) * m;
}

Time complexity: O(n/2)

int pow(int m, int n)
{
  if(n==0)
    return(1);
  if(n%2==0)
    return pow(m*m,n/2);
  else
    return m * pow(m * m, (n-1)/2);
}
