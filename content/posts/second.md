---
title: "Second blog test"
date: 2020-09-15T11:30:03+00:00
# weight: 1
# aliases: ["/first"]
tags: ["first"]
series: ["test"]
author: "Me"
mathjax: true
# author: ["Me", "You"] # multiple authors
draft: false
hideSummary: false
---

## second

*1234567*

When $a \ne 0$, there are two solutions to $ax^2 + bx + c = 0$ and they are: 

$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}$$


```rust
fn main() {
    // Declare vector with three values
    let three_nums = vec![15, 3, 46];
    println!("Initial vector: {:?}", three_nums);

    // Declare vector of length = 5, specify first element value = "0"
    // Short form of: let zeroes = vec!["0", "0", "0", "0", "0"]
    let zeroes = vec![0; 5];
    println!("Zeroes: {:?}", zeroes);

    // Create empty vector, make vector mutable so it can grow and shrink
    let mut fruit = Vec::new();

    // Push some values onto the end of the vector
    // Adding values changes the type from generic to the date type of the value: String
    fruit.push("Apple");
    fruit.push("Banana");
    fruit.push("Cherry");
    println!("Fruits: {:?}", fruit);

    // Push integer value, but vector expects String (&str) type value
    // REMOVE COMMENT SLASH MARKS to test
    // fruit.push(1); // returns error

    // Pop off value at end of vector
    // We can call the pop() method from inside the println! macro
    println!("Pop off: {:?}", fruit.pop());
    println!("Fruits: {:?}", fruit);

    // Declare vector with three values
    let mut index_vec = vec![15, 3, 46];
    let three = index_vec[1];
    println!("Vector: {:?}, three = {}", index_vec, three);

    // Add 5 to the value at index 1, 5 + 3 = 8
    index_vec[1] = index_vec[1] + 5;
    println!("Vector: {:?}", index_vec);

    // Try to access the vector with an out-of-bounds index = 10
    // Program compiles, but panics and stops at the invalid expression
    let beyond = index_vec[10];
    println!("Vector: {:?}, {}", index_vec, beyond);
}
```
