# leetcode
leet code activites
1. Palindrome Number
class Solution:
    def isPalindrome(self, x: int) -> bool:
        s = str(x)[::-1]
        return str(x) == s
2.reverseString
  class Solution:
    def reverseString(self, s: List[str]) -> None:
        s[:] = s[::-1]

         
