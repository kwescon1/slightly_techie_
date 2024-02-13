# ASSIGNMENT ONE

1. **Check if Even or Odd**:

   ```javascript
   const num = 4;
   console.log(num % 2 === 0 ? "Even" : "Odd");
   ```

2. **Favorite Fruits**:

   ```javascript
   const fruits = ["Apple", "Banana", "Cherry"];
   fruits.forEach((fruit) => console.log(fruit));
   ```

3. **Convert to Uppercase**:

   ```javascript
   const str = "hello";
   console.log(str.toUpperCase());
   ```

4. **Check Palindrome**:

   ```javascript
   const str = "madam";
   console.log(
     str === str.split("").reverse().join("")
       ? "Palindrome"
       : "Not a palindrome"
   );

   function isPalindrome(s) {
     let left = 0; // Start pointer
     let right = s.length - 1; // End pointer

     while (left < right) {
       if (s[left].toLowerCase() !== s[right].toLowerCase()) {
         return false; // Not a palindrome
       }
       left++; // Move the left pointer to the right
       right--; // Move the right pointer to the left
     }
     return true; // String is a palindrome
   }

   // Example usage:
   console.log(isPalindrome("A man, a plan, a canal: Panama")); // Returns false without alphanumeric filtering
   console.log(isPalindrome("madam")); // Returns true
   ```

5. **Declare Age Variable**:

   ```javascript
   const age = 30;
   console.log(`I am ${age} years old.`);
   ```

6. **Print Numbers 1 to 10**:

   ```javascript
   for (let i = 1; i <= 10; i++) {
     console.log(i);
   }
   ```

7. **Check Number Sign**:

   ```javascript
   const num = -5;
   console.log(num > 0 ? "Positive" : num < 0 ? "Negative" : "Zero");
   ```

8. **Convert to Lowercase**:

   ```javascript
   const str = "HELLO";
   console.log(str.toLowerCase());
   ```

9. **Sum of Array Elements**:

   ```javascript
   const numbers = [1, 2, 3, 4, 5];
   const sum = numbers.reduce((acc, num) => acc + num, 0);
   console.log(sum);
   ```

10. **Check Leap Year**:

    ```javascript
    const year = 2020;
    console.log(
      (year % 4 === 0 && year % 100 !== 0) || year % 400 === 0
        ? "Leap Year"
        : "Not a Leap Year"
    );
    ```

11. **Print Sum of Two Numbers**:

    ```javascript
    const num1 = 5,
      num2 = 10;
    console.log(num1 + num2);
    ```

12. **Message Based on Day of the Week**:

    ```javascript
    const day = "Monday";
    switch (day) {
      case "Monday":
        console.log("It's Monday!");
        break;
      // Add cases for other days...
      default:
        console.log("It's another day!");
    }
    ```

13. **Area of Rectangle**:

    ```javascript
    const length = 5,
      width = 10;
    console.log(length * width); // Area
    ```

14. **Convert String to Number**:

    ```javascript
    const str = "123.45";
    console.log(parseFloat(str));
    ```

15. **Check Name in Array**:

    ```javascript
    const names = ["Alice", "Bob", "Charlie"];
    const name = "Alice";
    console.log(names.includes(name) ? "Exists" : "Does not exist");
    ```

16. **Check Prime Number**:

    ```javascript
    const num = 7;
    let isPrime = num > 1;
    for (let i = 2; i <= Math.sqrt(num); i++) {
      if (num % i === 0) {
        isPrime = false;
        break;
      }
    }
    console.log(isPrime ? "Prime" : "Not prime");
    ```

17. **Boolean Check and Print**:

    ```javascript
    const isHarmattan = false;
    if (!isHarmattan) console.log("It's raining!");
    ```

18. **Print Even Numbers 1 to 20**:

    ```javascript
    for (let i = 1; i <= 20; i++) {
      if (i % 2 === 0) console.log(i);
    }
    ```

19. **Factorial of a Number**:

    ```javascript
    const factorial = (n) => (n <= 1 ? 1 : n * factorial(n - 1));
    console.log(factorial(5));
    ```

20. **Convert Number to String**:

    ```javascript
    const num = 123;
    console.log(num.toString());
    ```

21. **Print Length of Colors Array**:

    ```javascript
    const colors = ["red", "green", "blue"];
    console.log(colors.length);
    ```

22. **Check Valid Email**:

    ```javascript
    const email = "test@example.com";
    console.log(/^\S+@\S+\.\S+$/.test(email) ? "Valid" : "Invalid");
    ```

23. **Print Largest Number**:

    ```javascript
    const num1 = 10,
      num2 = 20,
      num3 = 15;
    console.log(Math.max(num1, num2, num3));
    ```

24. **Check Number Between Two Numbers**:

    ```javascript
    const num = 15,
      lower = 10,
      upper = 20;
    console.log(num > lower && num < upper);
    ```

25. **Convert Celsius to Fahrenheit**:

    ```javascript
    const celsius = 30;
    console.log((celsius * 9) / 5 + 32); // Fahrenheit
    ```

26. **Convert String "10" to Number**:

    ```javascript
    console.log(parseInt("10"));
    ```

27. **Declare Age Without Value**:

    ```javascript
    let age;
    ```

28. **Print Numbers 1 to 5**:

    ```javascript
    for (let i = 1; i <= 5; i++) {
      console.log(i);
    }
    ```

29. **Combine && and ||**:

    ```javascript
    const a = 5,
      b = 10,
      c = 15;
    if (a < b && (c > b || a < c)) console.log("True");
    ```

30. **Switch Statement for Day**:

    ```javascript
    const day = "Tuesday";
    switch (day) {
      case "Monday":
        console.log("Monday blues");
        break;
      case "Tuesday":
        console.log("Just Tuesday");
        break;
      // Add more cases as needed
      default:
        console.log("Another day");
    }
    ```

31. **Positive or Negative Number**:

    ```javascript
    const num = -5;
    console.log(num > 0 ? "Positive" : "Negative");
    ```

32. **Convert Number 5 to String**:

    ```javascript
    console.log(5.toString());
    ```

33. **Compare Two Numbers**:

    ```javascript
    const num1 = 10,
      num2 = 20;
    console.log(num1 > num2); // false
    ```

34. **Print Even Numbers 1 to 10**:

    ```javascript
    for (let i = 1; i <= 10; i++) {
      if (i % 2 === 0) console.log(i);
    }
    ```

35. **Combine && and !**:

    ```javascript
    const a = true,
      b = false;
    if (a && !b) console.log("True");
    ```

36. **Switch Statement for Month**:

    ```javascript
    const month = "February";
    switch (month) {
      case "January":
        console.log("January");
        break;
      case "February":
        console.log("February");
        break;
      // Add more cases as needed
      default:
        console.log("Another month");
    }
    ```

37. **Check Divisibility by 3**:

    ```javascript
    const num = 9;
    console.log(num % 3 === 0 ? "Divisible by 3" : "Not divisible by 3");
    ```

38. **Print Numbers 10 to 1**:

    ```javascript
    for (let i = 10; i >= 1; i--) {
      console.log(i);
    }
    ```

39. **Combine || and !**:

    ```javascript
    const a = false,
      b = true;
    if (a || !b) console.log("True");
    else console.log("False");
    ```

40. **Switch Statement for Season**:
    ```javascript
    const season = "Winter";
    switch (season) {
      case "Spring":
        console.log("It's Spring");
        break;
      case "Summer":
        console.log("It's Summer");
        break;
      case "Fall":
        console.log("It's Fall");
        break;
      case "Winter":
        console.log("It's Winter");
        break;
      default:
        console.log("Unknown season");
    }
    ```
