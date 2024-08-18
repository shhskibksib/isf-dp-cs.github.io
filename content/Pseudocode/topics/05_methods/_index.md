---
title: Methods
weight: 6
draft: true
---

# Methods

This page contains information and coding exercises for `methods`.

Open up the [pseudocode compiler](http://ibcomp.fis.edu/pseudocode/pcode.html) in a new tab. You will be using this website to complete the exercises below.


### Creating a Method
```java
method printNums(NUMS)
   loop C from 0 to 9
      output NUMS[C]
   end loopg
   output "========"
end method
```


## Practice Exercises

### Exercise 1: Looping

{{< code-action >}} **Create a method `search()` that checks for a certain number in a list**     
**Parameters:** a list of numbers,  a number to look for     
**Return:** True/False

1. Create a method that loops through a list
2. Receives a list of numbers as a parameter
3. Returns true if the number is in the list
4. Returns false if the number is not in the list 



### Exercise 2: Improving Sorting

{{< code-action "Create an method called `swap()` that can swap two numbers in an array" >}}     
**Parameters:** position1, position2, array        
**Return:** nothing
 
1. Swap the items at postition1 and postition1
2. Return the updated array

**Now use your `swap`` to improve your sorting**

{{< code-action "Create a method called `bubbleSort`" >}}     
**Parameter:** a list of numbers          
**Return:** a sorted list of numbers    
1. Sorts the list
2. Everytime a swap is required, it should use `swap()` 


## Deliverables

{{< deliverables >}}
Paste your code in your Exercises lab log

Complete the [Exit Ticket](https://docs.google.com/forms/d/e/1FAIpQLScgcYSCyOc-9A60yAu78deLLUhKunf9wPlE_D1hJHy12Hzq1Q/viewform?usp=sf_link)

{{< /deliverables >}}