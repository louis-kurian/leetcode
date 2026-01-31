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

3.class Solution:
    def romanToInt(self, s: str) -> int:
        roman={"I":1,"V":5,"X":10,"L":50,"C":100,"D":500,"M":1000}
        number=0
        for i in range(len(s)-1):
            if roman[s[i]] < roman[s[(i+1)]]:
                number-=roman[s[i]]
            else:
                number+=roman[s[i]]
        return number+roman[s[-1]]
         
