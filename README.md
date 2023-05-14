<!-- # LeetCode-7-code
LeetCode 07 Easy Code-->
class Solution {
public:
    int reverse(int x) {
        int ans=0;
        while(x!=0){
            int rem = x % 10;
            if(ans < (INT_MIN/10 )|| ans >( INT_MAX/10)) {
                return 0;
            }
            ans = 10 *ans + rem;
            x = x/10;
        }
        return ans;
    }
};
