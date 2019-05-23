# Collection Types

Swift provides three primary collection types, known as arrays, sets, and dictionaries, for storing collections of values. Arrays are ordered collections of values. Sets are unordered collections of unique values. Dictionaries are unordered collections of key-value associations.

## Array

Creating an Empty Array 

```swift

var someInts = [Int]()
var threeDoubles = Array(repeating: 0.0, count: 3)

```

## Sets

Creating and Initializing an Empty Set

```swift

var letters = Set<Character>()
letters.insert("a")
// letters now contains 1 value of type Character
letters = []
var favoriteGenres: Set<String> = ["Rock", "Classical", "Hip hop"]
var favoriteGenres: Set = ["Rock", "Classical", "Hip hop"]

```

## Dictionaries

Creating an Empty Dictionary

```swift
var namesOfIntegers = [Int: String]()
namesOfIntegers[16] = "sixteen"
// namesOfIntegers now contains 1 key-value pair
namesOfIntegers = [:]
// namesOfIntegers is once again an empty dictionary of type [Int: String]
var airports: [String: String] = ["YYZ": "Toronto Pearson", "DUB": "Dublin"]
var airports = ["YYZ": "Toronto Pearson", "DUB": "Dublin"]

```