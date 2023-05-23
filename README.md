# duplicate-number-coding-ninja-
You have been given an integer array/list(ARR) of size N which contains numbers from 0 to (N - 2). Each number is present at least once. There is a single integer value that is present twice. You need to find and return that duplicate number present in the array.
int duplicateNumber(int *arr, int size)
{
    int count=0;
   for(int i=0;i<size;i++)
   {
      int count=0;
     for (int j = 0; j < size; j++) {
         if(i==j)
         {
         continue;
         }
         if(*(arr + i)==*(arr + j))
         count++;
     }
     if (count == 1){
         int k=*(arr+i);
        return k;
     }
       
   }
}
