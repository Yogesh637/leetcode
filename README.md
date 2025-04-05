# leetcode
class Solution {
    public boolean canJump(int[] nums) {
        int fd = nums.length-1;
        for(int i = nums.length-2;i>=0;i--){
            if(i + nums[i] >= fd){
                fd =i;
            }
        }
        return fd == 0;
    }
}
