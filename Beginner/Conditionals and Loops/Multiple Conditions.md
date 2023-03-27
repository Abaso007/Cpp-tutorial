Combining Conditions
---
In some scenarios we need to combine multiple conditions. Let's say we want to check that the temp value is between 36 and 38.
This can be done using the && operator:
```
if(temp >= 36 && temp <= 38) {
  cout << "OK";
}
```
><font color="#AE8E00">The && operator is also referred to as the logical AND operator.</font>

---
OR
---
The logical OR operator, written as || combines conditions and checks if any one of them is true.
For example:
```
int level = 2;
int points = 321;
    
if(level > 5 || points > 200) {
  cout << "Welcome";
}
```

><font color="#AE8E00">The code above will output "Welcome" if the level value is greater than 5, or points is greater than 200.</font>
---
NOT
---
The logical NOT operator ! reverses the condition: in case the condition is true, the not operator will make it false, and vice-e-versa.
For example:
```
if(!(height < 150)) {
  cout << "Welcome";
}
```

><font color="#AE8E00">!(height < 150) means "if height is NOT less than 150".</font>

---
Multiple Conditions
---
You can chain multiple conditions using parentheses and the logical operators.
For example:
```
if((city == 'NY' || city == 'LA') && price < 100000) {
  cout << "Yes";
}
```
><font color="#AE8E00">You can chain as many conditions as you need.</font>
---
Lesson Takeaways
---
Logical operators allow you to combine multiple conditions.

- The AND operator && combines two conditions and checks if both of them are true.
- The OR operator || check if any of the conditions are true.
- The NOT operator ! reverses the condition.
- You can combine and chain conditions using parentheses and logical operators.
 

The next lesson will be fun! We will cover loops, which allow you to repeat a block of code.
