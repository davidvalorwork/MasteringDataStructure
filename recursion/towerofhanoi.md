# Tower of Hanoi using recursion

## C++

void TOH(int n, int a, int b, int c)
{
  if(n>0)
  {
    TOH(n-1, a, c, b);
    printf("from %d to %d", a, c);
    TOH(n-1,b,a,c);
  }
}
