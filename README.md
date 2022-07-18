# TIL
## Today what i learned !
 💻 📒📕 📗📘📙📚📖




### Variables and Constants
**변수와 상수**  
#### **var : 설정된 값을 변경할 수 있는 변수(가변 변수)**

var [변수명]: [데이터 타입] = [값]  변수 생성시 데이터 타입 생략 가능. 

```markdown
var name: String = "yjpotato"

var job: String = "ios programmer"

var fruit = "apple"
```

 👉 값을 변경할 때는 기존과 같은 타입의 값을 할당해주어야 한다.

#### **let : 설정된 값을 변경할 수 없는 상수(불변 변수)**

let [상수명]: [데이터 타입] = [값]  상수 생성시 데이터 타입 생략 가능. 

```markdown
let name: String = "yjpotato" 

let age: Int = 25

let height = 155
```

👉 상수로 선언된 값은 변경할 수 없다. 오류가 발생
### Data Types in Swift
**데이터 타입**
#### Numeric Type


유형을 지정하지 않으면 Swift의 유형 유추는 기본적으로 Double을 사용한다.

다음은 Double Type 값으로 상수를 선언하는 몇 가지 예입니다. 
```
let num = 15.2
type(of: num) // Double
```

첫 번째 경우, Swift 컴파일러는 자동으로 해당 유형을 Double로 유추한다.

Float 유형의 변수 또는 상수를 선언하려면, 이 예제와 같이 명시적 유형 주석을 사용해야 한다.
```
let num1 = 14.2
type(of: num1) // Float
```

##### Int와 UInt
Int : +, - 부호를 포함한 정수
UInt : - 부호를 포함하지 않는 0을 포함한 양의 정수
##### Bool
Bool은 불리언 타입이다. 불리언 타입은 참(true)또는 거짓(false)만 값으로 가진다.
```
var boolean: Bool = true
boolean.toggle()   // true-false 반전
```
true 또는 false는 따옴표 없이 작성된다.
부울은 조건문과 루프에서 매우 유용하게 이용된다.



#### Strings and Characters
##### String : 문자의 나열, 즉 문자열을 말한다. 
문자열은 큰 따옴표(“)로 묶어 표현 합니다.
```markdown
let fruit:String = "apple"
let name = "yoojin"
```
여러줄 문자열 리터럴
여러줄의 문자열을 사용하고 싶은 경우 큰 따옴표 3개(“””)로 묶어서 사용할 수 있다.
```
let Antoninus = """
The universe is change.
our life is what our thoughts make it.
"""
```
연산자를 통한 문자열 결합
```
let hello = "Hello"
let name = "yoojin"
var greeting = hello + "" + name
print(greeting) // Hello yoojin
```
문자열 안에서 큰 따옴표(“)를 표현하고 싶을 경우 ( \“ )로 묶어 표현한다.
```
"""
Adele – Someone Like You

\"I heard that you’re settled down
That you found a girl and you’re married now.
I heard that your dreams came true.
Guess she gave you things I didn’t give to you.\"
"""
```
##### Character : 유니코드에서 지원하는 모든 언어 및 특수기호.
문자는 큰 따옴표(“)로 묶어 표현 한다.
```
let book: Character = "📒"
let 한글변수이름: Character ="ㄱ"
// 한글도 유니코드 문자에 속하므로 스위프트 코드의 변수 이름으로 사용할 수 있으나 권장하지 않음.
```

#### Operators
**연산자**
```
연산자는 단항, 이항, 삼항, 전위, 중위, 후위 연산자로 구분된다.
A = B : 할당 연산자이며, A에 B라는 값을 '할당' 해준다.
A + B, - *, /, % : 산술연산자이며 수학 연산을 위한 기능을 제공한다.
A > B, <, ==, !=, ===(참조가 같다) : 비교 연산자이며, 참 거짓 여부를 반환한다.
A ? B : C : 삼항 조건 연산자이며 형태가 이거 하나이다. A가 참인 경우 B, 아닌 경우 C를 리턴한다.
A...B, A..<B, A..., ...A : 범위 연산자이며 값의 범위를 나타낸다.
A ?? B : nil병합 연산자이며 A가 nil인 경우 B를 반환한다.
```
#### Making Decisions
**조건문**
조건문에서는 if 구문과 switch 구문을 이용한다.
##### if
```
let first: Int = 5
let second: Int = 4

if first > second{
    print("first > second")
}else if first == second{
    print("first == second")
}else {
    print("first < second")
}
```
else if는 몇개가 이어져도 상관 없으며 else 블록은 없어도 상관 없다. 
맨위의 if문의 조건을 충족하지 않으면 다음 else if문의 명령을 실행하고, else if문의 조건을 충족하지 않으면 다음 else 문을 실행하게 된다.
##### switch
``` 
switch 입력 값 {
case 비교 값1:
     실행 구문
case 비교 값2:
     실행 구문
     //이번 case를 마치고 switch 구문을 탈출하지 않는다. 아래 case로 넘어감.
     fallthrough
case 비교 값3, 비교 값4, 비교 값5:  // 한번에 여러 값과 비교 가능.
     실행 구문
     break  // break 키워드를 통한 종료는 선택 사항.
default:    // 한전된 범위가 명확지 않다면 default는 필수.
     실행 구문     
}
```
**case XXX: 다음에는 꼭 실행 가능한 코드가 위치해야 한다.**
예시 (문자열 switch case 구성)
```
let stringValue: String = "Lian Neeson"

switch stringValue {
case "yoojin":
     print("She is yoojin")
case "Jay"   
     print("She is yoojin")
case "Jenny", "Joker", "Nova":
     print("He or She is \(stringValue)")
defalut:
     print("\(stringValue) said 'I don't know who you are'")
}
// Liam Neeson said  'I don't know who you are'
```
#### Repeating Tasks
**반복문**
##### for-in
for-in 반복 구문 ***은 반복적인 데이터나 시퀀스를 다룰 때 많이 사용한다.
```
for 임시 상수 in 시퀀스 아이템 {
    실행코드
}
```
예시 
```
for i in 0...2{
    print(i)
}
// 0
// 1
// 2
for i in 0...5{
    if i.isMultiple(of: 2) {
        print(i)
        continue   // continue 키워드를 사용하면 바로 다음 시퀀스로 건너뛴다.
    }
    print("\(i) == 홀수")
}

//0
// 1 == 홀수
// 2
// 3 == 홀수
// 4
// 5 == 홀수
```
💡 break문과 continue 차이점
break문은 조건문도 빠져나가면서 반복문 자체도 탈출하고 끝이나지만,
continue문은 해당 '조건문만' 실행하지 않고, 반복문은 이어서 실행하는 제어문이다.
##### while
while 반복문도 for-in과 마찬가지로 continue. break 등의 제어 키워드 사용이 가능하다.
```
var counter = 0
 
while counter <= 100 {
    print(counter)
    counter += 1
    
    if counter == 10{
        break
    }
    
}
print("stop")
//0
//1
.
.
.
//9
//stop

```
##### repeat - while
repeat - while 반복문은 다른 프로그래밍 언어의 do-while 구문과 크게 다르지 않다.
repeat 블록의 코드를 최초 1회 실행한 후, while 다음의 조건이 성립하면 블록 내부의 코드를 반복 실행한다.
```
var names: [String] = ["Jenny", "Joker", "yoojin"]

repeat {
    print("Good bye \(names.removeFirst())")
    // removeFirst()는 요소를 삭제함과 동시에 삭제한 요소를 반환한다.
} while names.isEmpty == false

// Good bye Jenny
// Good bye Joker
// Good bye yoojin
```

#### Functions
**함수**
```
func 함수 이름(매개 변수...) -> 반환 타입 {
    실행 구문
    return 반환 값
}
```
예시1
```
func river(jeong:Int, baeck:Int){
    if jeong == baeck{
        print("same")
    }else if jeong > baeck{
        print("jeong win")
    }else {
        print("baeck win")
    }
}
river(jeong: 56, baeck: 88)
// baeck win
```
예시2
```
func calcu(bil:Double) -> Double {
    let tip = bil * 0.1
    return tip
}
calcu(bil: 25.3)
let bil = 25.3
let squ = bil + calcu(bil: bil)
```

#### Collections
**배열**
```
// 대괄호를 사용하여 배열임을 표현.
var names: Array<String> = ["yoojin", "Jenny", "Joker"]
// 위 선언과 정확히 동일한 표현. [String]은 Array<String>의 축약 표현.
var names: [String] = ["yoojin", "Jenny", "Joker"]
var emptyArray: [Any] = [Any]() // Any 데이터를 요소로 갖는 빈 배열을 생성.
var emptyArray: [Any] = Array<Any>() // 위 선언과 정확히 같은 동작을 하는 코드

// 배열의 타입을 정확히 명시해줬다면 []만으로도 빈 배열을 생성할 수 있다.
var emptyArray: [Any] = []
print(emptyArray.isEmpty) // true
print(names.count)  // 4
```
배열의 사용
```
var names: Array<String> = ["yoojin", "Jenny", "Joker"]
names.append("elsa") // ["yoojin", "Jenny", "Joker", "elsa"]
names.insert("happy", at: 2) // ["yoojin", "Jenny","happy", "Joker", "elsa"]
names.removeFirst() // ["Jenny","happy", "Joker", "elsa"]
names.removeLast() // ["Jenny","happy", "Joker"]
print(names.firstIndex(of: "yagom"))  // nil
print(names.firstIndex(of: "Jenny"))  // 0 
```
**딕셔너리**
딕셔너리는 요소들이 순서 없이 키와 값의 쌍으로 구성되는 컬렉션 타입.
하나의 딕셔너리 안의 키는 같은 이름을 중복해서 사용할 수 없다.
```
// 키는 String, 값은 Int 타입인 빈 딕셔너리를 생성한다.
var numberForName: Dictionary<String, Int> = Dictionary<String, Int>()
// 위 선언과 같은 표현. [String: Int]는 Dictionary<String, Int>의 축약표현
var numberForName: [String: Int] = [String: Int]()
//위 코드와 같은 동작을 한다.
var numberForName: StringIntDictionary = StringIntDictionary()
// 딕셔너리의 키와 값 타입을 정확히 명시해줬다면 [:]만으로도 빈 딕셔너리를 생성할 수 있다.
var numberForName: [String: Int] = [:]
// 초깃값을 주어 생성해줄수도 있다.
var numberForName: [String: Int] = ["yagom":100. "yoojin":200, "Jenny":300]
print(numberForName.isEmpty) // false
print(numberForName.count)  //3
```
**세트**  

세트는 같은 타입의 데이터를 순서 없이 하나의 묶음으로 저장하는 형태의 컬렉션 타입이다.
세트 내의 값은 모두 유일한 값, 즉 중복된 값이 존재하지 않는다. 그래서 세트는 보통 **순서가
중요하지 않거나 각 요소가 유일한 값이어야 하는 경우**에 사용한다.

세트의 선언과 생성
```
var names: Set<String> = Set<String>() // 빈세트 생성
var names: Set<String> = []

//Array와 마찬가지로 대괄호를 사용한다.
var names: Set<String> = ["yagom", "yoojin", "jenny"]
```
세트의 사용
```
print(names.count)  // 3
print(names.remove("kai"))  // nil
```


