# TIL
## Today what i learned !
 π» ππ πππππ





### Variables and Constants


**λ³μμ μμ**  
#### **var : μ€μ λ κ°μ λ³κ²½ν  μ μλ λ³μ(κ°λ³ λ³μ)**

var [λ³μλͺ]: [λ°μ΄ν° νμ] = [κ°]  λ³μ μμ±μ λ°μ΄ν° νμ μλ΅ κ°λ₯. 

```markdown
var name: String = "yjpotato"

var job: String = "ios programmer"

var fruit = "apple"
```

Β πΒ κ°μ λ³κ²½ν  λλ κΈ°μ‘΄κ³Ό κ°μ νμμ κ°μ ν λΉν΄μ£Όμ΄μΌ νλ€.

#### **let : μ€μ λ κ°μ λ³κ²½ν  μ μλ μμ(λΆλ³ λ³μ)**

let [μμλͺ]: [λ°μ΄ν° νμ] = [κ°]  μμ μμ±μ λ°μ΄ν° νμ μλ΅ κ°λ₯. 

```markdown
let name: String = "yjpotato" 

let age: Int = 25

let height = 155
```

π μμλ‘ μ μΈλ κ°μ λ³κ²½ν  μ μλ€. μ€λ₯κ° λ°μ

### Data Types in Swift
**λ°μ΄ν° νμ**
#### Numeric Type


μ νμ μ§μ νμ§ μμΌλ©΄ Swiftμ μ ν μ μΆλ κΈ°λ³Έμ μΌλ‘ Doubleμ μ¬μ©νλ€.

λ€μμ Double Type κ°μΌλ‘ μμλ₯Ό μ μΈνλ λͺ κ°μ§ μμλλ€. 
```
let num = 15.2
type(of: num) // Double
```

μ²« λ²μ§Έ κ²½μ°, Swift μ»΄νμΌλ¬λ μλμΌλ‘ ν΄λΉ μ νμ Doubleλ‘ μ μΆνλ€.

Float μ νμ λ³μ λλ μμλ₯Ό μ μΈνλ €λ©΄, μ΄ μμ μ κ°μ΄ λͺμμ  μ ν μ£Όμμ μ¬μ©ν΄μΌ νλ€.
```
let num1 = 14.2
type(of: num1) // Float
```


##### Intμ UInt
Int : +, - λΆνΈλ₯Ό ν¬ν¨ν μ μ
UInt : - λΆνΈλ₯Ό ν¬ν¨νμ§ μλ 0μ ν¬ν¨ν μμ μ μ

##### Bool

Boolμ λΆλ¦¬μΈ νμμ΄λ€. λΆλ¦¬μΈ νμμ μ°Έ(true)λλ κ±°μ§(false)λ§ κ°μΌλ‘ κ°μ§λ€.
```
var boolean: Bool = true
boolean.toggle()   // true-false λ°μ 
```
true λλ falseλ λ°μ΄ν μμ΄ μμ±λλ€.
λΆμΈμ μ‘°κ±΄λ¬Έκ³Ό λ£¨νμμ λ§€μ° μ μ©νκ² μ΄μ©λλ€.




#### Strings and Characters
##### String : λ¬Έμμ λμ΄, μ¦ λ¬Έμμ΄μ λ§νλ€. 

λ¬Έμμ΄μ ν° λ°μ΄ν(β)λ‘ λ¬Άμ΄ νν ν©λλ€.
```markdown
let fruit:String = "apple"
let name = "yoojin"
```
μ¬λ¬μ€ λ¬Έμμ΄ λ¦¬ν°λ΄
μ¬λ¬μ€μ λ¬Έμμ΄μ μ¬μ©νκ³  μΆμ κ²½μ° ν° λ°μ΄ν 3κ°(βββ)λ‘ λ¬Άμ΄μ μ¬μ©ν  μ μλ€.
```
let Antoninus = """
The universe is change.
our life is what our thoughts make it.
"""
```
μ°μ°μλ₯Ό ν΅ν λ¬Έμμ΄ κ²°ν©
```
let hello = "Hello"
let name = "yoojin"
var greeting = hello + "" + name
print(greeting) // Hello yoojin
```
λ¬Έμμ΄ μμμ ν° λ°μ΄ν(β)λ₯Ό νννκ³  μΆμ κ²½μ° ( \β )λ‘ λ¬Άμ΄ νννλ€.
```
"""
Adele β Someone Like You

\"I heard that youβre settled down
That you found a girl and youβre married now.
I heard that your dreams came true.
Guess she gave you things I didnβt give to you.\"
"""
```

##### Character : μ λμ½λμμ μ§μνλ λͺ¨λ  μΈμ΄ λ° νΉμκΈ°νΈ.

λ¬Έμλ ν° λ°μ΄ν(β)λ‘ λ¬Άμ΄ νν νλ€.
```
let book: Character = "π"
let νκΈλ³μμ΄λ¦: Character ="γ±"
// νκΈλ μ λμ½λ λ¬Έμμ μνλ―λ‘ μ€μννΈ μ½λμ λ³μ μ΄λ¦μΌλ‘ μ¬μ©ν  μ μμΌλ κΆμ₯νμ§ μμ.
```


#### Operators



**μ°μ°μ**
```
μ°μ°μλ λ¨ν­, μ΄ν­, μΌν­, μ μ, μ€μ, νμ μ°μ°μλ‘ κ΅¬λΆλλ€.
A = B : ν λΉ μ°μ°μμ΄λ©°, Aμ BλΌλ κ°μ 'ν λΉ' ν΄μ€λ€.
A + B, - *, /, % : μ°μ μ°μ°μμ΄λ©° μν μ°μ°μ μν κΈ°λ₯μ μ κ³΅νλ€.
A > B, <, ==, !=, ===(μ°Έμ‘°κ° κ°λ€) : λΉκ΅ μ°μ°μμ΄λ©°, μ°Έ κ±°μ§ μ¬λΆλ₯Ό λ°ννλ€.
A ? B : C : μΌν­ μ‘°κ±΄ μ°μ°μμ΄λ©° ννκ° μ΄κ±° νλμ΄λ€. Aκ° μ°ΈμΈ κ²½μ° B, μλ κ²½μ° Cλ₯Ό λ¦¬ν΄νλ€.
A...B, A..<B, A..., ...A : λ²μ μ°μ°μμ΄λ©° κ°μ λ²μλ₯Ό λνλΈλ€.
A ?? B : nilλ³ν© μ°μ°μμ΄λ©° Aκ° nilμΈ κ²½μ° Bλ₯Ό λ°ννλ€.
```


#### Making Decisions
**μ‘°κ±΄λ¬Έ**
μ‘°κ±΄λ¬Έμμλ if κ΅¬λ¬Έκ³Ό switch κ΅¬λ¬Έμ μ΄μ©νλ€.
#### ifλ¬Έ


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
else ifλ λͺκ°κ° μ΄μ΄μ Έλ μκ΄ μμΌλ©° else λΈλ‘μ μμ΄λ μκ΄ μλ€. 
λ§¨μμ ifλ¬Έμ μ‘°κ±΄μ μΆ©μ‘±νμ§ μμΌλ©΄ λ€μ else ifλ¬Έμ λͺλ Ήμ μ€ννκ³ , else ifλ¬Έμ μ‘°κ±΄μ μΆ©μ‘±νμ§ μμΌλ©΄ λ€μ else λ¬Έμ μ€ννκ² λλ€.



##### switch

``` 
switch μλ ₯ κ° {
case λΉκ΅ κ°1:
     μ€ν κ΅¬λ¬Έ
case λΉκ΅ κ°2:
     μ€ν κ΅¬λ¬Έ
     //μ΄λ² caseλ₯Ό λ§μΉκ³  switch κ΅¬λ¬Έμ νμΆνμ§ μλλ€. μλ caseλ‘ λμ΄κ°.
     fallthrough
case λΉκ΅ κ°3, λΉκ΅ κ°4, λΉκ΅ κ°5:  // νλ²μ μ¬λ¬ κ°κ³Ό λΉκ΅ κ°λ₯.
     μ€ν κ΅¬λ¬Έ
     break  // break ν€μλλ₯Ό ν΅ν μ’λ£λ μ ν μ¬ν­.
default:    // νμ λ λ²μκ° λͺνμ§ μλ€λ©΄ defaultλ νμ.
     μ€ν κ΅¬λ¬Έ     
}
```

#### Guard
```
guard μ‘°κ±΄ else {
	//μ‘°κ±΄μ΄ falseλ©΄ μ€ν
    return || throw
}
```


**case XXX: λ€μμλ κΌ­ μ€ν κ°λ₯ν μ½λκ° μμΉν΄μΌ νλ€.**
μμ (λ¬Έμμ΄ switch case κ΅¬μ±)
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
**λ°λ³΅λ¬Έ**
##### for-in


for-in λ°λ³΅ κ΅¬λ¬Έ ***μ λ°λ³΅μ μΈ λ°μ΄ν°λ μνμ€λ₯Ό λ€λ£° λ λ§μ΄ μ¬μ©νλ€.
```
for μμ μμ in μνμ€ μμ΄ν {
    μ€νμ½λ
}
```
μμ 
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
        continue   // continue ν€μλλ₯Ό μ¬μ©νλ©΄ λ°λ‘ λ€μ μνμ€λ‘ κ±΄λλ΄λ€.
    }
    print("\(i) == νμ")
}

//0
// 1 == νμ
// 2
// 3 == νμ
// 4
// 5 == νμ
```
π‘ breakλ¬Έκ³Ό continue μ°¨μ΄μ 
breakλ¬Έμ μ‘°κ±΄λ¬Έλ λΉ μ Έλκ°λ©΄μ λ°λ³΅λ¬Έ μμ²΄λ νμΆνκ³  λμ΄λμ§λ§,
continueλ¬Έμ ν΄λΉ 'μ‘°κ±΄λ¬Έλ§' μ€ννμ§ μκ³ , λ°λ³΅λ¬Έμ μ΄μ΄μ μ€ννλ μ μ΄λ¬Έμ΄λ€.



##### while

while λ°λ³΅λ¬Έλ for-inκ³Ό λ§μ°¬κ°μ§λ‘ continue. break λ±μ μ μ΄ ν€μλ μ¬μ©μ΄ κ°λ₯νλ€.
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

repeat - while λ°λ³΅λ¬Έμ λ€λ₯Έ νλ‘κ·Έλλ° μΈμ΄μ do-while κ΅¬λ¬Έκ³Ό ν¬κ² λ€λ₯΄μ§ μλ€.
repeat λΈλ‘μ μ½λλ₯Ό μ΅μ΄ 1ν μ€νν ν, while λ€μμ μ‘°κ±΄μ΄ μ±λ¦½νλ©΄ λΈλ‘ λ΄λΆμ μ½λλ₯Ό λ°λ³΅ μ€ννλ€.
```
var names: [String] = ["Jenny", "Joker", "yoojin"]

repeat {
    print("Good bye \(names.removeFirst())")
    // removeFirst()λ μμλ₯Ό μ­μ ν¨κ³Ό λμμ μ­μ ν μμλ₯Ό λ°ννλ€.
} while names.isEmpty == false

// Good bye Jenny
// Good bye Joker
// Good bye yoojin
```



### Functions

**ν¨μ**
```
func ν¨μ μ΄λ¦(λ§€κ° λ³μ...) -> λ°ν νμ {
    μ€ν κ΅¬λ¬Έ
    return λ°ν κ°
}
```
μμ1
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
μμ2
```
func calcu(bil:Double) -> Double {
    let tip = bil * 0.1
    return tip
}
calcu(bil: 25.3)
let bil = 25.3
let squ = bil + calcu(bil: bil)
```


### Collections

### Array

**λ°°μ΄**
```
// λκ΄νΈλ₯Ό μ¬μ©νμ¬ λ°°μ΄μμ νν.
var names: Array<String> = ["yoojin", "Jenny", "Joker"]
// μ μ μΈκ³Ό μ νν λμΌν νν. [String]μ Array<String>μ μΆμ½ νν.
var names: [String] = ["yoojin", "Jenny", "Joker"]
var emptyArray: [Any] = [Any]() // Any λ°μ΄ν°λ₯Ό μμλ‘ κ°λ λΉ λ°°μ΄μ μμ±.
var emptyArray: [Any] = Array<Any>() // μ μ μΈκ³Ό μ νν κ°μ λμμ νλ μ½λ

// λ°°μ΄μ νμμ μ νν λͺμν΄μ€¬λ€λ©΄ []λ§μΌλ‘λ λΉ λ°°μ΄μ μμ±ν  μ μλ€.
var emptyArray: [Any] = []
print(emptyArray.isEmpty) // true
print(names.count)  // 4
```
λ°°μ΄μ μ¬μ©
```
var names: Array<String> = ["yoojin", "Jenny", "Joker"]
names.append("elsa") // ["yoojin", "Jenny", "Joker", "elsa"]
names.insert("happy", at: 2) // ["yoojin", "Jenny","happy", "Joker", "elsa"]
names.removeFirst() // ["Jenny","happy", "Joker", "elsa"]
names.removeLast() // ["Jenny","happy", "Joker"]
print(names.firstIndex(of: "yagom"))  // nil
print(names.firstIndex(of: "Jenny"))  // 0 
```
#### Ditionary
**λμλλ¦¬**

λμλλ¦¬λ μμλ€μ΄ μμ μμ΄ ν€μ κ°μ μμΌλ‘ κ΅¬μ±λλ μ»¬λ μ νμ.
νλμ λμλλ¦¬ μμ ν€λ κ°μ μ΄λ¦μ μ€λ³΅ν΄μ μ¬μ©ν  μ μλ€.
```
// ν€λ String, κ°μ Int νμμΈ λΉ λμλλ¦¬λ₯Ό μμ±νλ€.
var numberForName: Dictionary<String, Int> = Dictionary<String, Int>()
// μ μ μΈκ³Ό κ°μ νν. [String: Int]λ Dictionary<String, Int>μ μΆμ½νν
var numberForName: [String: Int] = [String: Int]()
//μ μ½λμ κ°μ λμμ νλ€.
var numberForName: StringIntDictionary = StringIntDictionary()
// λμλλ¦¬μ ν€μ κ° νμμ μ νν λͺμν΄μ€¬λ€λ©΄ [:]λ§μΌλ‘λ λΉ λμλλ¦¬λ₯Ό μμ±ν  μ μλ€.
var numberForName: [String: Int] = [:]
// μ΄κΉκ°μ μ£Όμ΄ μμ±ν΄μ€μλ μλ€.
var numberForName: [String: Int] = ["yagom":100. "yoojin":200, "Jenny":300]
print(numberForName.isEmpty) // false
print(numberForName.count)  //3
```

#### set

**μΈνΈ**  


μΈνΈλ κ°μ νμμ λ°μ΄ν°λ₯Ό μμ μμ΄ νλμ λ¬ΆμμΌλ‘ μ μ₯νλ ννμ μ»¬λ μ νμμ΄λ€.
μΈνΈ λ΄μ κ°μ λͺ¨λ μ μΌν κ°, μ¦ μ€λ³΅λ κ°μ΄ μ‘΄μ¬νμ§ μλλ€. κ·Έλμ μΈνΈλ λ³΄ν΅ **μμκ°
μ€μνμ§ μκ±°λ κ° μμκ° μ μΌν κ°μ΄μ΄μΌ νλ κ²½μ°**μ μ¬μ©νλ€.

μΈνΈμ μ μΈκ³Ό μμ±
```
var names: Set<String> = Set<String>() // λΉμΈνΈ μμ±
var names: Set<String> = []

//Arrayμ λ§μ°¬κ°μ§λ‘ λκ΄νΈλ₯Ό μ¬μ©νλ€.
var names: Set<String> = ["yagom", "yoojin", "jenny"]
```
μΈνΈμ μ¬μ©
```
print(names.count)  // 3
print(names.remove("kai"))  // nil
```

#### Class & Struct
##### class
ν΄λμ€λ μ°Έμ‘°  νμ
ν΄λμ€λ ν΄λμ€λΌλ¦¬ μμμ΄ κ°λ₯νλ€!
```
class myIntroduce {
    var name = "yoojin"
    
    func my_name() {
        print("my name is \(name)")
    }
}

let jyj : myIntroduce = myIntroduce()

print(jyj.name)
jyj.my_name()

jyj.name = "Jeong"
jyj.my_name()

// yoojin
my name is yoojin
my name is Jeong
```
##### struct
κ΅¬μ‘°μ²΄λ κ° νμ
```
struct Sqaure {
    let length: Double
    
    func calculateArea(){
        length * length
        print(calculateArea)
    }
    
}
```
## class μ struct κ³΅ν΅μ 

- κ°μ μ μ₯νκΈ° μν νλ‘νΌν°λ₯Ό μ μν  μ μμ
- κΈ°λ₯μ μ κ³΅νκΈ° μν΄ λ©μλλ₯Ό μ μν  μ μμ
## class μ struct μ°¨μ΄μ 
### class

- μ°Έμ‘° νμ
- ARCλ‘ λ©λͺ¨λ¦¬ κ΄λ¦¬
- κ°μ ν΄λμ€ μΈμ€ν΄μ€λ₯Ό μ¬λ¬ κ° λ³μμ ν λΉν λ€ κ°μ λ³κ²½μν€λ©΄ ν λΉν λͺ¨λ  λ³μμ μν₯μ μ€
- μμ κ°λ₯(ν΄λμ€λΌλ¦¬)

### struct

- κ° νμ
- κ΅¬μ‘°μ²΄ λ³μλ₯Ό μλ‘μ΄ λ³μμ ν λΉν  λλ§λ€ μλ‘μ΄ κ΅¬μ‘°μ²΄κ° ν λΉ
- κ°μ λ³κ²½μν€λλΌλ λ€λ₯Έ λ³μμ μν₯μ μ£Όμ§ μμ

## enum
enumμ μμκ°μ΄ μλ μ΄κ±°νμ΄λ€.
```
enum fruit {
case apple, watermelon, banana
}
```
νλμ caseλ₯Ό μ΄μ©ν΄μ λμ΄ν΄μ μμ±ν  μ μλ κ°λμ±μ΄ μλ€.

πΒ μμκ°μ΄ μλ μ΄κ±°ν!
```
enum school{
    case elementary
    case middle
    case high

}
let yourschool = school.middle
print("myschool",yourschool)

enum grade: Int{
    case first = 1
    case second = 2
    
}
let yourgrade = grade.second
let yourgrade = grade.second.rawValue 
print("my grade: \(yourgrade)")
print("my grade: \(yourgrade.rawValue)") 
```

#### κ΅¬μ‘°μ²΄

# Optionals

nilμ λ³μ λλ μμμ κ°μ΄ μμ μ μλ€ λΌλ λ»μΌλ‘ ν΄μνλ©΄ μ’λ€.

μ΅μλμ ν΄μ ν  μ μλ λ°©λ²μ μ΄ 3κ°μ§

# μ΅μλ λ°μΈλ©

μ΅μλ λ°μΈλ©μ μ£Όλ‘ if let(λλ if var)κ΅¬λ¬Έκ³Ό κ°μ΄ μ°μΈλ€.
λ¨Όμ  μ²΄ν¬ν΄μ€λ€! λΌκ³  μκ°νλ©΄ μ΄ν΄νκΈ° μ½λ€.

μ΄κ² nilμΈμ§, μλλ©΄ κ°μ΄ μλμ§,κ²½μ°μ λ°λΌ κ²°κ³Όλ₯Ό λ¬λ¦¬ νκ³  μΆμ μ μμλ, μ΅μλ λ°μΈλ©μ μ¬μ©νμ¬ κ²μ¬ν΄μ£Όλ©΄ λλ€.

μ΅μλ μ²΄μ΄λ

κ°μ  μΈλ©ν

μ°Έκ³   : Swift5[μΌκ³°]
     : https://www.udemy.com/course/swift-5-for-absolute-beginners/learn/lecture/28626408#overview
     
