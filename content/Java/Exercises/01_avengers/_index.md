---
title: "0. Avengers"
weight: 10
# draft: true
---

# Avengers

## [0] Create the Avengers class based on the specs below


|   <center>**Avengers**</center>  |
|:------------------------|
  | **--Properties--** |
| - name: String    |
| - alias: String   |
| - age: int        |
| - powers: LinkedList\<String\> |
  | **--Methods--** |
| + Avengers(String name, String alias, int age, LinkedList\<String\> powers) |
| + getName(): returns a String |
| + setName(String name): returns void |
| + getAlias(): returns a String |
| + setAlias(String alias): returnsvoid |
| + getAge(): returns an int |
| + setAge(int age): returns void |
| + getPowers(): returns a LinkedList\<String\> |
| + addPower(String power): returns void |
| + removePower(String power): returns void |
| + printInfo(): returns void | 
  
 The `printInfo()` method should print out all the attributes, including each power
  
----

 ## [1] Test your Avengers Class

  1. Create a  `main()` method that creates an avenger, `avenger1` .
  2. Change the attributes of `avenger1` using your setters
  2. Print the updated information of `avenger1`
  3. Create a second avenger and print their information
