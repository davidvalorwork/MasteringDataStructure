# Binary Search using Arrays

## C++ loop

Time complexity: Best O(1) Worst P(logN)

BinSearch(l,h,key)
{
  while(l<=h)
  {
    mid = [(l+h)/2];
    if(key == a[mid])
      return mid;
    else if(key < a[mid])
      h=mid-1;
    else
      l=mid+1;
  }
  return -1
}

## C++ recursive

Time complexity: Best O(1) Worst P(logN)

RBinSearch(l,h,key)
{
  if(l <= h)
  {
    mid=[(l+h)/2];
    if(key == a[mid])
      return mid;
    else if (key<a[mid])
      return RBinSearch(l,mid-1,key);
    else 
      return RBinSearch(mid+1,h,key);
  }
}
