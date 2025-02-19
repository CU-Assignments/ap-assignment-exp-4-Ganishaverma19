# experiment-no.-4-22BCS_IOT-701B
```bash
https://leetcode.com/problems/longest-nice-substring/description/

class Solution {
public:
 bool check(string s){
        for(int i=0;i<s.size();i++) {
            char c = s[i];
            if(c<=90) c += 32;
            else c -= 32;
            if(s.find(c)==string::npos) return false;
        }
        return true;
    }
    string longestNiceSubstring(string s) {
        string ans = "";
        for(int i=0;i<s.size();i++){
            string res = "";
            res += s[i];
            for(int j = i+1;j<s.size();j++){
                res += s[j];
                if(check(res) and res.size()>ans.size()) ans = res;
            }
        }
        return ans;
    }
};

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

