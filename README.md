# Java Tutorials

### 1. Hello World Program
**Task:**
- Write a simple Java program that prints `Hello, World!` to the console.

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

---

### 2. Variables and Data Types
**Task:**
- Declare and initialize different types of variables: `int`, `double`, `char`, `boolean`, `String`.

```java
public class VariablesExample {
    public static void main(String[] args) {
        int age = 25;
        double height = 5.9;
        char grade = 'A';
        boolean isJavaFun = true;
        String name = "John Doe";
        
        System.out.println("Age: " + age);
        System.out.println("Height: " + height);
        System.out.println("Grade: " + grade);
        System.out.println("Is Java fun? " + isJavaFun);
        System.out.println("Name: " + name);
    }
}
```

---

### 3. User Input
**Task:**
- Take user input using `Scanner` and print the input value.

```java
import java.util.Scanner;

public class UserInputExample {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Enter your name: ");
        String name = scanner.nextLine();
        
        System.out.println("Hello, " + name + "!");
        
        scanner.close();
    }
}
```

---

### 4. If-Else Condition
**Task:**
- Write a Java program that checks if a number is even or odd.

```java
import java.util.Scanner;

public class EvenOddChecker {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Enter a number: ");
        int number = scanner.nextInt();
        
        if (number % 2 == 0) {
            System.out.println("The number is even.");
        } else {
            System.out.println("The number is odd.");
        }
        
        scanner.close();
    }
}
```

---

### 5. Loops (For Loop)
**Task:**
- Print numbers from 1 to 10 using a `for` loop.

```java
public class ForLoopExample {
    public static void main(String[] args) {
        for (int i = 1; i <= 10; i++) {
            System.out.println(i);
        }
    }
}
```

---

### 6. Loops (While Loop)
**Task:**
- Print numbers from 10 to 1 using a `while` loop.

```java
public class WhileLoopExample {
    public static void main(String[] args) {
        int i = 10;
        while (i >= 1) {
            System.out.println(i);
            i--;
        }
    }
}
```

---

### 7. Arrays
**Task:**
- Declare an integer array and print all elements.

```java
public class ArrayExample {
    public static void main(String[] args) {
        int[] numbers = {10, 20, 30, 40, 50};
        
        for (int num : numbers) {
            System.out.println(num);
        }
    }
}
```

---

### 8. Functions (Methods)
**Task:**
- Write a method that takes two numbers and returns their sum.

```java
public class MethodExample {
    public static int add(int a, int b) {
        return a + b;
    }

    public static void main(String[] args) {
        int sum = add(5, 10);
        System.out.println("Sum: " + sum);
    }
}
```

---

### 9. Switch Case
**Task:**
- Write a program that takes an integer input (1-3) and prints a message based on the value.

```java
import java.util.Scanner;

public class SwitchExample {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Enter a number (1-3): ");
        int choice = scanner.nextInt();
        
        switch (choice) {
            case 1:
                System.out.println("You selected One.");
                break;
            case 2:
                System.out.println("You selected Two.");
                break;
            case 3:
                System.out.println("You selected Three.");
                break;
            default:
                System.out.println("Invalid selection.");
        }
        
        scanner.close();
    }
}
```

---

### 10. Exception Handling
**Task:**
- Implement try-catch to handle division by zero.

```java
import java.util.Scanner;

public class ExceptionHandlingExample {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        try {
            System.out.print("Enter numerator: ");
            int numerator = scanner.nextInt();
            
            System.out.print("Enter denominator: ");
            int denominator = scanner.nextInt();
            
            int result = numerator / denominator;
            System.out.println("Result: " + result);
        } catch (ArithmeticException e) {
            System.out.println("Error: Division by zero is not allowed.");
        } finally {
            scanner.close();
        }
    }
}
```

---

## Bonus Challenge 💡
**Create a Java program that calculates the factorial of a number using recursion.**
- Write a method `factorial(int n)` that returns `n!`.
- Call the method in `main()` and print the result.

---


