class Solution {
    public int[] smallerNumbersThanCurrent(int[] nums) {
        int arr[]=new int[nums.length];
        for(int i=0;i<nums.length;i++)
        {
            int length=0;
            int num=nums[i];//8
            for(int j=0;j<nums.length;j++)
            {
                if(num-nums[j]>0&&num!=nums[j])//8
                {
                    length=length+1;//4
                }
            }
            arr[i]=length;//[4,0,1,1,3]
        }
        return arr;//[4,0,1,1,3]
    }
}
