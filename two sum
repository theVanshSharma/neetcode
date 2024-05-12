Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

You can return the answer in any order.

// vector<int>result;
        // int n= nums.size();
        // for(int i=0;i<n;i++){
        //     int complement = target-nums[i];
        //     int j=0;
        //     while(j<n){
        //         if(nums[j]==complement){
        //             result.push_back(i);
        //             result.push_back(j);
        //         }
        //     }
        // }
        // return result;
        
        // vector<int> result;
        // int n= nums.size();
        // for(int i=0;i<n;i++){
        //     for(int j=i+1;j<n;j++){
        //         if((nums[i]+nums[j])==target){
        //             result.push_back(min(i,j));
        //             result.push_back(max(i,j));
        //             break;
        //         }
        //     }
        // }
        // return result;

        int n = nums.size();
        unordered_map<int, int> mp; // val -> index

        for (int i = 0; i < n; i++) {
            int complement = target - nums[i];
            if (mp.find(complement) != mp.end()) {
                return {mp[complement], i};
            }
            mp.insert({nums[i], i});
        }
        return {};
