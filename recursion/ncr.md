# NCR with Recursion

## C++ using pascal triangle

Time complexity: 

int c(int n, int r)
{
  if(r==0 || n ==r)
    return 1;
  return c(n-1,r-1) + c(n-1,r);
}
