# BASIC

## Constants and Variables

let 是常量， var是变量 “，”号分割
可以声明类型.有了值类型后就不能改了。。（静态语言）

字符串模版  \\()

## Comments

// 

/*.....*/ 这个注解可以嵌套

## Semicolons

不需要;号

## Number

1.25e2 意味着 1.25 * 10平方

数字可以用_扩充，以易于阅读 比如1_000_000

Int8 (-128-127) UInt8 (0-255) 需要类型转换，如同python
浮点数不会四舍五入化整，直接切割取整数部分

## Type Aliases

就是声明类型太麻烦了，你可以提供一个昵称，这是一个关键字

typealias Audio = UInt16

var x = Audio.min

## Tuple

支持直接写field名称 let http200Status = (statusCode: 200, description: "OK")

## Optionals

You use optionals in situations where a value may be absent. An optional represents two possibilities: Either there is a value, and you can unwrap the optional to access that value, or there isn’t a value at all.
当一个值可能缺失的情况下，你可以使用optionals这个语法

语法 a: Int? = 5
如果不赋值 比如 a :Int?
a的值为nil
nil只有在optionals情况下才能赋值给变量，否则不可以，nil不是指针，而是值的意思it’s the absence of a value of a certain type. Optionals of any type can be set to nil, not just object types.

ou can access its underlying value by adding an exclamation mark (!) to the end of the optional’s name. The exclamation mark effectively says, “I know that this optional definitely has a value; please use it.” This is known as forced unwrapping of the optional’s value:

if convertedNumber != nil {
    print("convertedNumber has an integer value of \(convertedNumber!).")
}

if let actualNumber = Int(possibleNumber) {
    print("The string \"\(possibleNumber)\" has an integer value of \(actualNumber)")
} else {
    print("The string \"\(possibleNumber)\" could not be converted to an integer")
}
// Prints "The string "123" has an integer value of 123"

This code can be read as:
如果这个的int转换包含一个值，把它的值赋给actual，否则走别的分支
“If the optional Int returned by Int(possibleNumber) contains a value, set a new constant called actualNumber to the value contained in the optional.”
还可以写多行版本的

if let firstNumber = Int("4"), let secondNumber = Int("42"), firstNumber < secondNumber && secondNumber < 100 {
    print("\(firstNumber) < \(secondNumber) < 100")
}
// Prints "4 < 42 < 100"

if let firstNumber = Int("4") {
    if let secondNumber = Int("42") {
        if firstNumber < secondNumber && secondNumber < 100 {
            print("\(firstNumber) < \(secondNumber) < 100")
        }
    }
}
// Prints "4 < 42 < 100"

String?是问号，！是默认有值





