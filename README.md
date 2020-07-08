# kotlin-basics
This repo contains kotlin snippets to learn basics. The code is inspired from raywenderlich's kotlin cheat sheet.


### kotlin variables

```kotlin
// Declaring a variable
var subscriberCount: Int = 1
subscriberCount = 2 //okay

// Declaring immutable variable
// You can't reassign it
val likes: Int = 10
likes = 11 //error

/*
  Nullable variable
  description can be string or null
  ? specifies that a variable is nullable
*/ 
var description: String? = null
description = "Learning kotlin variables"
```

### Control-flow : If expression

```kotlin
var admin = true

if (admin) {
  // if condition is true, this block is executed
} else {
  // else block, if condition is false
}

val a = 10
val b = 11

// Using if to set a value
val equal = if (a==b) true else false
```

### Control-flow : when expression

```kotlin
// when is equivalent to switch in java

var platform = "Instagram"

when (platform) {
  "Instagram" -> print("Founded in 2010")
  "Youtube" -> printf("Founded in 2005")
  else -> print("Wrong platform")
}

// using when to set a value
val ceo = when {
  platform == "Instagram" -> "Kevin Systrom"
  platform == "Youtube" -> "Susan Wojcicki"
  else -> "No CEO"
}
```

### Control-flow : for loops

```kotlin

// iterate over a list or set
for (value in listOrSet) {
  println(value)
}

// iterate over a map
for ((key, value) in demoMap) {
  println("$key : $value")
}

// simple for loop counters
for (i in 0..10) {} // 0 to 10
for (i in 0 until 10) {} // 0 to 9
```
