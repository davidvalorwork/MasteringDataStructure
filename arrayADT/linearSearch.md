# Linear Search in array

## C++

for(i=0;i<length;i++)
{
  if(key==A[i])
    return i;
}
return -1;

## C++ transposition

for(i=0;i<length;i++)
{
  if(key==A[i]){
    swap(A[i],A[i-1])
    return i-1;
  }
}
return -1;

## C++ move to front/head

for(i=0;i<length;i++)
{
  if(key==A[i]){
    swap(A[i],A[0])
    return 0;
  }
}
return -1;
