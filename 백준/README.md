## 백준 알고리즘
[https://www.acmicpc.net/](https://www.acmicpc.net/)


### **전체문제**
- [1000](#1000)
- [1001](#1001)


### **알고리즘 분류**
- 


### **필요한 개념**
- [readLine](#readLine)
- [split](#split)


***
### **[전체문제]**

### 1000
```swift
//1000

let A = Int(readLine()!) ?? 0
let B = Int(readLine()!) ?? 0
print(A+B)

```
문제는 tool에서는 아무런 이상이 없는 데 백준에서는 런타임 에러남... 
애플이 맞겠거니 싶음,,(통과하려면 아래 1001번 문제에서 print(a+b)로만 바꿔주면 통과함...)

이것때문에 시간 오지게 버림...... (첫문제부터 백준을 해야하나?... 의구심이 들었음)

### 1001
```swift
let line = readLine() ?? "" 
let Arr = line.split{$0 == " "}.map(String.init) 
let a = Int(Arr[0]) ?? 0 
let b = Int(Arr[1]) ?? 0 

print(a-b)
```
문제는 백준은 통과하는데 tool에서는 **Thread 1: Fatal error: Index out of range**라고 에러뜸... -.,-


***
### **[필요한 개념]** 
### readLine
[https://developer.apple.com/documentation/swift/1641199-readline](https://developer.apple.com/documentation/swift/1641199-readline)
- Foundation영향을 받지 않는다. 
- 입력값에 대한 입출력을 도와준다. 
예) 1000(A+B)으로 예시를 들면, 
![](image/read2.png)
a는 readLine()에 대한 문자열 값을 받는다(b와 동일)
pirnt는 (a+b)로 출력되어 testtest1가 된다.
![](image/read1.png)
모 이런식임..
*Int로 반환할 경우*
![](image/read.png)


### split
- 특정 문자시, 단위로 쪼개줌.
- 단, map을 꼭 써야함. 
예시)
![](image/map.png)


### 


