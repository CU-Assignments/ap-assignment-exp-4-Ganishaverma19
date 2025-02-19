# experiment-no.-4-22BCS_IOT-701B
```bash
https://leetcode.com/problems/longest-nice-substring/description/

https://leetcode.com/problems/maximum-subarray/description/
class Solution {
public:
   int maxSubArray(std::vector<int>& nums)
    {
      int n = nums.size();
      int maxsum = INT_MIN;
      for(int  start = 0;start <n;start++) 
      {
        int currsum =0 ;
         for(int end=start;end<n;end++)
         { 
          currsum += nums[end];
           maxsum = max(maxsum,currsum);
         }  

        }
      return maxsum;
    }
};
Experiment no. 4
```

