In JavaScript, you can use the `Date` object to get the current date and time. Here are a few ways to do it:

1. **Using the `Date()` constructor**:
```
const currentDate = new Date();
console.log(currentDate); // Output: Current date and time
```
This will give you an instance of the `Date` object, which contains various methods for working with dates.

2. **Using the `toISOString()` method**:
```
const dateString = new Date().toISOString();
console.log(dateString); // Output: A string in ISO format (e.g., "2023-03-15T14:30:00.000Z")
```
This will give you a string representation of the current date and time in the ISO format.

3. **Using the `getFullYear()`, `getMonth()`, and `getDate()` methods**:
```
const year = new Date().getFullYear();
const month = new Date().getMonth(); // Month is 0-based (January=0, February=1, etc.)
const day = new Date().getDate();
console.log(`${year}-${month+1}-${day}`); // Output: Current date in the format "YYYY-MM-DD"
```
These methods allow you to extract specific parts of the current date.

4. **Using the `toLocaleDateString()` method**:
```
const dateString = new Date().toLocaleDateString();
console.log(dateString); // Output: A string representation of the current date in the user's locale (e.g., "March 15, 2023")
```
This will give you a string representation of the current date in the format used by the user's locale.

Remember that JavaScript dates are represented as UTC (Coordinated Universal Time) by default. If you want to work with dates in a specific timezone, you'll need to adjust the date accordingly.