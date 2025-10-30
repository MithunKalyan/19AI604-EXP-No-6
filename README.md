## Experiment 6 – Create an Application to Demonstrate Vector Collection Object  

<H3>ENTER YOUR NAME:</H3>  
<H3>ENTER YOUR REGISTER NO:</H3>  
<H3>EX.NO.4</H3>  
<H3>DATE:</H3>  

<H1 ALIGN =CENTER> Demonstrating Vector Collection in Rust </H1>  

## AIM:  
To create a Rust application that demonstrates the use of the Vector (Vec) collection object.  

## EQUIPMENTS REQUIRED:  
- Hardware – PCs  
- Software – Visual Studio Code (Version 1.104.0)  
- Rust Installation  

## RELATED THEORETICAL CONCEPT:  

*Vectors in Rust:*  
A Vector (`Vec<T>`) is a growable array type in Rust. Unlike arrays, vectors can change their size at runtime by adding or removing elements.  

*Key Features of Vectors:*  
- Store a collection of values of the same type.  
- Grow dynamically as elements are inserted.  
- Provide indexing and safe element access using `.get()`.  
- Can be traversed using loops and iterators.  

## ALGORITHM:  
STEP 1: Start the program. <BR>  
STEP 2: Import the standard library (no external crates required). <BR>  
STEP 3: Define the `main` function. <BR>  
STEP 4: Create a new Vector using `Vec::new()` or the `vec![]` macro. <BR>  
STEP 5: Insert values into the vector using `.push(value)`. <BR>  
STEP 6: Iterate and print the elements of the vector. <BR>  
STEP 7: Access elements using indexing and `.get(index)`. <BR>  
STEP 8: End the program. <BR>  

## PROGRAM:  
```
// Rust program to demonstrate Vector Collection

fn main() {
    // Step 4: Create a new Vector
    let mut numbers: Vec<i32> = Vec::new();

    // Step 5: Insert values into the vector
    numbers.push(10);
    numbers.push(20);
    numbers.push(30);
    numbers.push(40);
    numbers.push(50);

    // Step 6: Iterate and print elements of the vector
    println!("Elements of the vector:");
    for num in &numbers {
        println!("{}", num);
    }

    // Step 7: Access elements using indexing and .get()
    println!("\nAccessing elements:");
    println!("First element (using index): {}", numbers[0]);
    
    match numbers.get(2) {
        Some(value) => println!("Third element (using get): {}", value),
        None => println!("No element found at index 2"),
    }

    // Demonstrate removing the last element
    numbers.pop();
    println!("\nAfter removing the last element:");
    for num in &numbers {
        println!("{}", num);
    }
}

```
## OUTPUT:

<img width="1183" height="987" alt="image" src="https://github.com/user-attachments/assets/d513d738-d49c-49d4-be40-b5cdc7184f99" />

<img width="502" height="281" alt="image" src="https://github.com/user-attachments/assets/c5d02b60-ac81-4211-b476-ecff14cc57f2" />

## RESULT:

Thus, the Rust program to demonstrate the Vector Collection Object was successfully implemented and executed.
