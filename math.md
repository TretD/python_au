# Math

+ [Reverse Integer](#reverse-integer)
+ [Palindrome Number](#palindrome-number)
+ [Fizz Buzz](#fizz-buzz)
+ [Fibonacci Number](#fibonacci-number)
+ [Largest Perimeter Triangle](#largest-perimeter-triangle)
+ [Sqrt(x)](#sqrtx)
+ [Base 7](#base-7)

## 504.Base 7

https://leetcode.com/problems/base-7/

```python
def convertToBase7(self, num: int) -> str:
    l, n = [], num < 0
    if n: num *= -1
    while num: 
        l.append(str(num % 7))
        num //= 7
    if n: l.append('-')    
    return ''.join(l[::-1])
    return [[]]
```

## 69.Sqrt(x)

https://leetcode.com/problems/sqrtx/

```python
def mySqrt(self, x: int) -> int:
    import math
    return(round(math.sqrt(x)))
    return [[]]
```

## 976.Largest Perimeter Triangle

https://leetcode.com/problems/largest-perimeter-triangle/

```python
def largestPerimeter(self, A: List[int]) -> int:
    for i in range(3,len(A)+1):
        if(A[i-3] < A[i-2] + A[i-1]):
            return sum(A[i-3:i])
    return 0
    return [[]]
```

## 509.Fibonacci Number

https://leetcode.com/problems/fibonacci-number/

```python
def fib(self, N: int) -> int:
    if N==0:
        return(n)
    elif N==1:
            return(n)
    elif exp:
        return((N-1)+(N-2))
    result=fib(N)
    return(result)
    return [[]]
```

## 412.Fizz Buzz

https://leetcode.com/problems/fizz-buzz/

```python
def fizzBuzz(self, n: int) -> List[str]:
    a=[]
    for i in range(1, n+1):
        if i % 3 == 0 and i % 5 == 0:
           a.append('FizzBuzz')
        elif i % 3 == 0:
            a.append('Fizz')
        elif i % 5 == 0:
            a.append('Buzz')
        else:
            a.append(str(i))
    return(a)
    return [[]]
```

## 9.Palindrome Number

https://leetcode.com/problems/palindrome-number/

```python
def isPalindrome(self, x: int) -> bool:
    L=list()
    LR=L.reverse()
    if L==LR:
        return('true')
    else:
        return('false')
    return [[]]
```

## 7.Reverse Integer

https://leetcode.com/problems/reverse-integer/

```python
def reverse(self, x: int) -> int:
    x = str(x)
    if x[0]!="-":
        x = x[::-1]
        if -2**31<=int(x)<=2**31-1:
            return int(x)
        else:
            return 0
    else:
        neg_symbol = x[0]
        x = x[1:]
        x = x[::-1]
        ans = neg_symbol+x
        if -2**31<=int(ans)<=2**31-1:
            return int(ans)
        else:
            return 0
     return [[]]
```