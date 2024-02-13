# ASSIGNMENT 2

1. **Concatenate Two Arrays**:

   ```javascript
   const concatenateArrays = (arr1, arr2) => [...arr1, ...arr2];
   ```

2. **Create "person" Object**:

   ```javascript
   const person = {
     name: "John Doe",
     age: 30,
     occupation: "Software Developer",
   };
   ```

3. **Check if Number is Even or Odd**:

   ```javascript
   const isEvenOrOdd = (num) => (num % 2 === 0 ? "Even" : "Odd");
   ```

4. **Double Each Element in an Array**:

   ```javascript
   const doubleElements = (arr) => arr.map((num) => num * 2);
   ```

5. **Capitalize First Letter of Each Word**:

   ```javascript
   const capitalizeWords = (words) =>
     words.map((word) => word.charAt(0).toUpperCase() + word.slice(1));
   ```

6. **Sum of All Elements in an Array**:

   ```javascript
   const sumElements = (arr) => arr.reduce((acc, num) => acc + num, 0);
   ```

7. **Sum an Arbitrary Number of Arguments**:

   ```javascript
   const sum = (...args) => args.reduce((acc, num) => acc + num, 0);
   ```

8. **Access Property Using `this` Keyword**:

   ```javascript
   function accessProperty() {
     return this.property;
   }
   const obj = { property: "value", accessProperty };
   console.log(obj.accessProperty()); // "value"
   ```

9. **Create "car" Object**:

   ```javascript
   const car = {
     make: "Toyota",
     model: "Corolla",
     year: 2020,
   };
   ```

10. **Copy of an Array**:

    ```javascript
    const copyArray = (originalArray) => [...originalArray];
    ```

11. **Check if Number is Positive, Negative, or Zero**:

    ```javascript
    const checkNumber = (num) =>
      num > 0 ? "Positive" : num < 0 ? "Negative" : "Zero";
    ```

12. **Convert Array of Strings to Uppercase**:

    ```javascript
    const toUpperCaseArray = (arr) => arr.map((str) => str.toUpperCase());
    ```

13. **Return Strings Containing Specific Substring**:

    ```javascript
    const filterBySubstring = (arr, substring) =>
      arr.filter((str) => str.includes(substring));
    ```

14. **Find Maximum Value in an Array**:

    ```javascript
    const findMax = (arr) =>
      arr.reduce((max, num) => (num > max ? num : max), arr[0]);
    ```

15. **Iterate Over Keys of an Object**:

    ```javascript
    const printKeys = (obj) => {
      for (let key in obj) {
        console.log(key);
      }
    };
    ```

16. **Concatenate Arbitrary Number of Strings**:

    ```javascript
    const concatenateStrings = (...strings) => strings.join("");
    ```

17. **Use `this` Keyword to Call a Method**:

    ```javascript
    const obj = {
      property: "value",
      method() {
        console.log(this.property);
      },
    };
    obj.method(); // "value"
    ```

18. **Create "book" Object**:

    ```javascript
    const book = {
      title: "The Great Gatsby",
      author: "F. Scott Fitzgerald",
      publicationYear: 1925,
    };
    ```

19. **Merge Two Objects**:

    ```javascript
    const mergeObjects = (obj1, obj2) => ({ ...obj1, ...obj2 });
    ```

20. **Check if String is Empty**:

    ```javascript
    const isEmptyString = (str) => (str === "" ? "Empty" : "Not Empty");
    ```

21. **Calculate Square of Each Element in an Array**:

    ```javascript
    const squareElements = (arr) => arr.map((num) => num ** 2);
    ```

22. **Return Numbers Divisible by a Specific Value**:

    ```javascript
    const filterDivisible = (arr, divisor) =>
      arr.filter((num) => num % divisor === 0);
    ```

23. **Find Average Value of an Array**:

    ```javascript
    const findAverage = (arr) =>
      arr.reduce((acc, num) => acc + num, 0) / arr.length;
    ```

24. **Iterate Over Words of a String**:

    ```javascript
    const printWords = (str) => {
      for (let word of str.split(" ")) {
        console.log(word);
      }
    };
    ```

25. \*\*Find Maximum Value in Arguments

\*\*:
`javascript
    const findMaxValue = (...nums) => Math.max(...nums);
    `

26. **Update Property Using `this` Keyword**:
    ```javascript
    const updateProperty = function (newValue) {
      this.property = newValue;
    };
    const obj = { property: "initial value", updateProperty };
    obj.updateProperty("updated value");
    console.log(obj.property); // "updated value"
    ```
