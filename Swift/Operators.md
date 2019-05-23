# Basic Operators

## Terminology

+ Unary operators operate on a single target (such as -a). Unary prefix operators appear immediately before their target (such as !b), and unary postfix operators appear immediately after their target (such as c!).
+ Binary operators operate on two targets (such as 2 + 3) and are infix because they appear in between their two targets.
+ Ternary operators operate on three targets. Like C, Swift has only one ternary operator, the ternary conditional operator (a ? b : c).

## Comparison Operators

!You can compare two tuples 
("blue", -1) < ("purple", 1)        // OK, evaluates to true
("blue", false) < ("purple", true)  // Error because < can't compare Boolean values

## Nil-Coalescing Operator

空值的缩写
原本这样的a != nil ? a! : b
改成 var colorNameToUse = userDefinedColorName ?? defaultColorName

## Range Operators

The closed range operator (a...b) defines a range that runs from a to b, and includes the values a and b.
...展开，范围 比如 1...5 就是1-5

The half-open range operator (a..<b) defines a range that runs from a to b, but doesn’t include b.  比如 1..<5

The closed range operator (a...b) defines a range that runs from a to b, and includes the values a and b.
比如[3..]或者[..6]或者[..<2]