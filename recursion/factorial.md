# Factorial of a Number

## C++

int fact(int n)
{
  if(n===0)
    return(1);
  else
    return fact(n-1)*n;
}
