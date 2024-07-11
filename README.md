# First-Missing-Positive

class Solution {
    public int firstMissingPositive(int[] nums) {
        int missingNumber =1;
        Arrays.sort(nums);
        for(int number : nums){
            if(number >0){
                if(number ==missingNumber){
                    missingNumber++;
                }
                else if(number>missingNumber){
                    break;
                }
            }
           
        }
         return missingNumber;
    }
}
*/
Input: nums = [1,2,0]
Output: 3
Explanation: The numbers in the range [1,2] are all in the array.
Input: nums = [7,8,9,11,12]
Output: 1
Explanation: The smallest positive integer 1 is missing.
 
/*

