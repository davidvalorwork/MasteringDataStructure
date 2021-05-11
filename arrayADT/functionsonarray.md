# Get() Set() Avg() Max()

## C++ 

Time complexity: O(1)

function Get(index)
{
  if(index >= 0 && index < length)
    return A[index]
}

Time complexity: O(1)

function Set(index,x)
{
  if(index >= 0 && index < length)
    return A[index] = x
}

Time complexity: O(n)

function Max()
{
  int max;
  max = A[0];
  for(i=1; i < length; i++) 
  {
    if(A[i] > max)
      max = A[i];
  }
  return max;
}

Time complexity: O(n)

function avg()
{
  total = 0;
  for(i = 0; i< length; i++)
  {
    total = total + A[i];
  }
  return total/n;
}
