# Taylor Series in Recursion

## C++

Time complexity: O(n^2)

int e(int x, int n)
{
  static int p=1, f=1;
  int r;
  if(n==0)
    return(1);
  else
  {
    r = e(x,n-1);
    p = p * x;
    f = f * n;
    return r + p/f;
  }
}

## C++ Horner's Rule

Time complexity: O(n)

int e(int x, int n)
{
  static int s = 1;
  if(n==0)
    return s;
  s = 1 + x / n * s;
  return e( x, n - 1)
}
