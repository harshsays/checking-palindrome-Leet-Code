# checking-palindrome-Leet-Code
Given an integer x, return true if x is a 
palindrome
, and false otherwise.

 

Example 1:

Input: x = 121
Output: true
Explanation: 121 reads as 121 from left to right and from right to left.
Example 2:

Input: x = -121
Output: false
Explanation: From left to right, it reads -121. From right to left, it becomes 121-. Therefore it is not a palindrome.
Example 3:

Input: x = 10
Output: false
Explanation: Reads 01 from right to left. Therefore it is not a palindrome.


______________________________________________________________________________________________________________________________________________________________________________


class Solution {
    public boolean isPalindrome(int x) {
       if (x <0) {
            return false;
        }
        int left=x;
        int total=0;
        while(left!=0){
            
            int remainder=left%10;
            int quotient=left/10;
            left=quotient;
            total=(total*10)+remainder;

        }
       return (total==x);
    } 
    }





 
