---
title: Collections
weight: 5
draft: true

---

# Collections

This page contains information and coding exercises for `collections`.

{{< code-action >}} Open up the [pseudocode compiler](http://ibcomp.fis.edu/pseudocode/pcode.html) in a new tab. You will be using this website to complete the exercises below.

## Examples of how to use Collections

### Creating a new Collection
```java
NAMES = new Collection()
```
### Adding to Collections
```java
NAMES.addItem("Bob")
NAMES.addItem("Dave")
NAMES.addItem("Betty")
NAMES.addItem("Kim")
NAMES.addItem("Debbie")
NAMES.addItem("Lucy")
```

### Important collection methods
```java
MYCOLLECTION.resetNext() // sets you at the beginning of the collection
MYCOLLECTION.hasNext() // checks if you are at the end of the collection. returns true/false
MYCOLLECTION.getNext() // moves to the next item in the collection. returns the next item
MYCOLLECTION.contains(THING) // checks if a thing is in the collection
MYCOLLECTION.remove(THING) // removes a thing to the collection
```

### Looping through a Collection

```java
// Using an while loop with an array
MYCOLLECTION.resetNext()
loop while MYCOLLECTION.hasNext()
    THING = MYCOLLECTION.getNext()
    output NAME
end loop
```

## Practice Exercises

### Exercise 1: Typhoon Warning System

{{< code-action "Write a program that determines the warning signal based on windspeed" >}}
  1. Create a collection
  2. Add 10 windspeeds to it
  3. Loop through the collection  
  4. For each windspeed, tell the user which signal is hoisted  

| Code | Windspeed| 
|:-----|:------------------|
| T3 | 41-62 km/h | 
| T8 | 63-117 km/h |
| T10+ | 118 km/h or more| 

Here is an example output:

```shell
T3
T8
T8
T3
T3
T8
T10+
T8
T8
T3
```

{{< code-action "Now add in a variable to keep track of the hour. Output the hour along with the typhoon signal." >}}

```shell
Hour 1 T3
Hour 2 T8
Hour 3 T8
Hour 4 T3
Hour 5 T3
Hour 6 T8
Hour 7 T10+
Hour 8 T8
Hour 9 T8
Hour 10 T3
```

 Reminder: you can print multiple things on one line using a comma
```shell
FRIEND = Jacob
output "hello", FRIEND
```

### Exercise 2: Dividing Teams

{{< code-action "Create two teams of students by alternating through the collection of names" >}}
  1. Create a collection
  2. Add 10 students to it
  3. Output team one
  4. Output team two

Here is an example:
```java
STUDENTS = new Collection()
STUDENTS.addItem("Bob")
STUDENTS.addItem("Dave")
STUDENTS.addItem("Betty")
STUDENTS.addItem("Kim")
STUDENTS.addItem("Debbie")
STUDENTS.addItem("Lucy")
```

output:
```java
TEAM 1
- Bob
- Betty
- Debby
-------
TEAM 2
- Dave
- Kim
- Lucy
```
