---
Title: 'Euclidean algorithm'
Description: 'A simple and efficient method for finding the highest common factor (HCF), also known as the greatest common divisor (GCD), of two numbers.'
Subjects:
  - 'Computer Science'
Tags:
  - 'Algorithms'
  - 'Arithmetic'
CatalogContent:
  - 'paths/computer-science'
---

The `Euclidean algorithm` is a recursive algorithm that allows developers to find the highest common factor (HCF) of two numbers. It is based on the observation that if two numbers are given, say A and B, where B divides A evenly (leaving no remainder), then B is the HCF of A and B. In other words, the larger number is divisible by the smaller number without any remainder.

There can be multiple methods to solve and find the highest common factor (HCF) of two numbers. In this explanation, let's explore a basic approach first and then move on to the `Euclidean algorithm`.

## Method 1

In the basic approach, the purpose is to find the GCD. To do this, find the minimum value between the two given numbers. Then, divide it by both numbers. If the number does not divide both numbers evenly, decrease it by `1` and continue dividing. Lastly, repeat this process until the minimum value can divide both numbers evenly. At this point, the minimum value is the HCF (highest common factor).

```java
public static void main(String[] args) {
        System.out.println(gcd(10,15));
    }
    public static int gcd(int a,int b){
        int minValue = Math.min(a,b);
        while(minValue>0){
            if(a%minValue==0 && b%minValue==0){
                break;
            }
            minValue--;
        }
        return minValue;
    }
}
```

The output for the above code will be:

```shell
5
```

## Approach with Euclidean algorithm

Here two methods are shown using Euclidean algorithm to find the HCF of two numbers. So let's take two numbers as 'a' and 'b' as our inputs.

## Method 2

In this method, the aim is to compare both 'a' and 'b'. Whichever number is greater,  the smaller number is subtracted from the larger number. It also updates the value of the larger number accordingly. If 'a' is greater than 'b', replace 'a' with 'a - b', and if 'b' is greater than 'a', replace 'b' with 'b - a'. Repeat this step until 'a' becomes equal to 'b'. Once 'a' and 'b' are equal, return 'a' as the answer. At this point, the value of 'a' (which is equal to 'b') represents the highest common factor (HCF) of the original values of 'a' and 'b'.

```java
class Euclidean1 {
static int gcd(int a, int b) {

    while (a != b) {
        if (a > b)
            a = a - b;
        else
            b = b - a;
    }

    return a;
}

public static void main(String[] args) {

    int a = 15, b = 20;

    System.out.println(gcd(a, b));

}
}
```

The output for the above code will be:

```shell
5
```

When debugging the code above step by step, one can analyze the code as follows:

- Since 'b' is greater than 'a' (20 > 15), here 'b' is replaced with 'b - a', which gives us 'b = 20 - 15 = 5'.
- Now 'a' is 15 and 'b' is 5.
- The result is 'a= 15-5=10' after replacing 'a' with 'a-b'.
- The values are now 'a = 10' and 'b = 5'.
- The process is continued as 'a' is replaced with 'a - b', resulting in 'a = 10 - 5 = 5'.
- Now 'a' and 'b' are both equal to 5.
- At this point, the while loop exits, and we return 'a' as our answer, which is 5.
- Therefore, the highest common factor (HCF) of (15, 20) is 5.

## Method 3

In this method, a recursive approach is used to implement the Euclidean algorithm for finding the greatest common divisor (GCD) of two integers, 'a' and 'b'. The method takes 'a' and 'b' as integer parameters and returns an integer as the result. The GCD method starts by checking if 'b' is equal to 0. If it is, then it means that 'a' is the GCD, and it returns 'a' as the result. However, if 'b' is not 0, it indicates that there is a remainder when 'a' is divided by 'b'. In this case, the method calls itself recursively with the arguments 'b' and 'a % b'. This recursive call continues until 'b' eventually becomes 0, triggering the base case and resulting in the discovery of the GCD.

For more information on recursion, refer to this [resource](https://www.codecademy.com/learn/java-algorithms/modules/recursion-apcs/cheatsheet).

```java
public class Euclidean2 {
public static void main(String[] args) {
    System.out.println(EuclideanOptimized(150, 500));

}
static int EuclideanOptimized(int a, int b){
    if(b==0){
        return a;
    }
    return EuclideanOptimized(b,a%b);
}
}
```

The output for the above code will be:

```shell
50
```

Let's debug the code above step by steps:

- Given the input of two integers: `a = 150` and `b = 500`, the code proceeds to enter the `EuclideanOptimized` function. The first `if` statement encountered checks if `b` is equal to 0. In this particular case, `b` is not equal to 0, resulting in the program exiting the `if` statement.
- Then the code proceeds to return `EuclideanOptimized`, but with the arguments changed to `(b, a % b)`.
- In the first recursive cycle, the value of `a % b` will be `150`. Since 150 is smaller than 500, it cannot be divided evenly by 500. Therefore, the remainder is equal to the original number, which is 150. Consequently, the next arguments for `EuclideanOptimized` are `(500, 150)`.
- The function is restarted with the arguments `(500, 150)`. Upon entering the function, the `if` statement is encountered. However, since `b` is not equal to 0, the program exits the `if` statement. The next recursive cycle will use the arguments `(150, 50)`, which are obtained by calculating the modulus of `500 % 150`.
- Once again, the function is initiated with arguments `(150, 50)`. Upon entering the function, the `if` statement is encountered. Similarly to previous iterations, `b` is not equal to 0, and thus the program exits the `if` statement. The new arguments for the next recursive cycle are determined by calculating the modulus of `150 % 50`, resulting in `(50, 0)`.
- In this recursive cycle, when the code enters the `if` statement, the condition `b == 0` is satisfied. Therefore, the function will return `a`, and the highest common factor (HCF) for the input will be 50.

## Time complexities

- Method 1:

  - The first code uses a simple iterative approach to find the greatest common divisor (GCD) of two numbers. It starts by finding the minimum value between `a` and `b`, then iterates from that value down to 1, checking if it divides both `a` and `b`. Therefore, the time complexity of this code is **O(min(a, b))**.

- Method 2:

  - The second code also calculates the GCD using an iterative approach known as the Euclidean algorithm. It repeatedly subtracts the smaller number from the larger number until the two numbers become equal (the GCD). The time complexity of this algorithm depends on the number of iterations required to reach the GCD. In the worst case, where one number is a multiple of the other, the time complexity is **O(max(a, b))**.

- Method 3:

  - The third code is an optimized version of the Euclidean algorithm that uses recursion. It calculates the GCD by repeatedly taking the modulus of `a` with `b` and calling itself with the new values (`b` and `a%b`) until `b` becomes 0. The time complexity of this optimized Euclidean algorithm is also O(log(max(a, b))) since the algorithm reduces the values quickly by taking the modulus.

To summarize, the time complexities of the three codes are as follows:

- Code 1: O(min(a, b))
- Code 2: O(max(a, b))
- Code 3: O(log(max(a, b)))

These time complexities typically represent the worst-case scenarios and assume that the `a` and `b` values are relatively large. In practice, the actual time taken by the algorithms can vary depending on the input values.
