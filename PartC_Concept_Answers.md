# Part C — Concept Answers

## 1. String immutability
A Java `String` cannot be changed after it is created. Operations such as concatenation create a new String instead of modifying the old one. Repeated modifications can create many temporary objects and waste time and memory. Use `StringBuilder` for repeated changes, especially inside loops.

## 2. The `this` keyword
`this` refers to the current object. If a constructor parameter has the same name as an instance field, `this.field` refers to the field while the bare name refers to the parameter.
```java
class Student {
    String name;
    Student(String name) {
        this.name = name;
    }
}
```

## 3. Object vs reference variable
An object is the instance stored in memory; a reference variable holds a value that refers to that object. Assigning `w2 = w1` copies the reference, not the object, so both variables can access the same object. Mutating it through either reference is visible through both.

## 4. Static vs instance variables
A `static` variable belongs to the class and is shared by all instances, such as a visitor counter. An instance variable belongs to one object, such as each student's name or each wallet's balance. Use static state for shared class-level data and instance state for per-object data.

## 5. `for`, `while`, and `do-while`
A `for` loop suits a known or count-controlled number of repetitions, such as iterating over an array. A `while` loop suits repetition while a condition remains true, such as reading until a sentinel value. A `do-while` loop executes its body at least once, making it suitable for a menu that must be displayed before checking whether the user wants to continue.

## 6. Pass-by-value
Java always passes arguments by value. For a primitive, the method receives a copy of the primitive, so reassigning the parameter does not change the caller's variable. For an object, the copied value is a reference; the method can mutate the referenced object, but reassigning the local parameter does not change the caller's reference.

## 7. Integer division
When both operands are integers, Java integer division discards the fractional part: `250 / 3` is `83`. To get a floating-point result, at least one operand must be floating-point, for example `250.0 / 3` or `(double) 250 / 3`.

## 8. Encapsulation
Encapsulation keeps an object's data and methods together and restricts direct access to internal state. Declaring fields `private` and providing controlled getters/setters lets a class validate changes and protect invariants, such as rejecting a negative balance.

## 9. `==` vs `equals()`
For object references, `==` checks whether both references point to the same object. `equals()` checks logical equality as defined by the class; `String` overrides it to compare character contents. A custom class can override `equals()` to compare meaningful fields rather than object identity.

## 10. Overloading vs overriding
Overloading uses the same method name with different parameter lists in the same class or inheritance context; the compiler selects the matching signature at compile time. Overriding occurs when a subclass provides a new implementation of an inherited method with the same signature; the implementation is selected at runtime based on the actual object type.
