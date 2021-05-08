# Combination Formula using recursion

## C++

Time complexity: O(n)

int C(int n, int r)
{
  int t1, t2, t3;
  t1 = fact(n);
  t2 = fact(r);
  t3 = fact(n-r);
  return t1/(t2 * t3);
}
