# Sort-colors

void sortColors(int* nums, int numsSize){
    int count0=0;
    int count1=0;
    int count2=0;
    int i;
    
    for(i=0;i<numsSize;++i)
    {
        if(nums[i]==0) count0++;
        else if(nums[i]==1) count1++;
        else count2++;
    }
    i=0;
    while(count0 !=0){
        nums[i]=0;
        i++;
        count0--;
    }
     while(count1 !=0){
        nums[i]=1;
         i++;
        count1--;
     }
     while(count2 !=0){
        nums[i]=2;
         i++;
        count2--;
     }
}
