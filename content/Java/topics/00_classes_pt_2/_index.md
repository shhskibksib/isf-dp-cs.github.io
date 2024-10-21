---
title: "OOP pt. 2" 
bookFlatSection: false
weight: 3
# bookCollapseSection: true
# draft: true
---

# OOP Part 2

---

## [0] Melee

Today's lab will build on the code from last class. 

{{< code-action >}} open up your **`lab_oop_yourgithubusername`** repository in IntelliJ

---

### Add Melee class

{{< code-action >}} **Make new class `Melee` inside the `model` package**

- Right-click on the package `model`
- Select `new > Java class`
- Name the class `Melee`
- Add the class to `git` when IntelliJ prompts you

---

### Main Method
{{< code-action >}} **Add a `main()` method to `Melee`.** 
Main methods **always** have the same declaration:

```java
public static void main(String[] args) 
```

- `public`: this means it can be accessed outside of this class
- `static`: this means this method belongs to the whole class, not just one particular object
- `void`: this means it will not return anything
- `String[] args`: this means that this method can accept parameters from the user

{{< code-action >}} **Create 4 `Superhuman` objects in the `main()` method.**

Since  they are in the same model, `Melee` can access the `Superhuman` class. However, it can only access attributes/methods that have the `public` access modifier.   

Because the `main()` method is `static`, we can run it even before we have created a constructor for `Melee`.


**Be sure to test our your `main()` method to make sure it's working before moving on!**

---

### Attributes and Constructor

{{< code-action >}} **Add the following attributes to the `Melee` class.**
 - `villains`: a java `array` of size 20, that holds `Superhuman` objects
 - `heroes`: a java `array` of size 20, that holds `Superhuman` objects
 - villainPoints: int        
 - heroPoints: int    

 You can use Java arrays like this:
 ```java
int[] array = new int[20]; //create an array of integers
array[0] = 8; //adds the integer 8 at index 0
 ```

{{< code-action >}} **Add the `constructor`.**
The constructor method is the method that runs when a new object is created. Remember, the constructor method must have the **same name as the class**. Take a look at the constructor from the other classes for inspiration.

The `Melee` constructor should takes no parameters. It creates `villains` and `heroes`. It sets both`villainPoints` and `heroPoints` to zero. 

**Constructors automatically return an object of their class, so you don't need any return statement**

---

## [1] Fight

We want to make it so that two of the superhumans can fight. However, first we need to know how what power the superhuman has, and how strong they are:

{{< code-action >}} **Add three attributes: `strength`, `powers`, and `isVillain`  to the `Superhuman` class.**

`strength`: an `int` that stores how powerful they are
`powers`: a `Strings` that stores the name of their power
`isVillain`: a `boolean` that stores whether the super is a villain or not.

You will also need to update:
- The `Superhuman` constructor to include parameters for the new attributes
- Create `accessors` and `mutators`  *(`getters`/`setters`)* for the new attributes
- Update any `Superhuman` objects that you create to include these new attributes

{{< code-action >}} **Add a method `fight()` to the `Melee` class.**

- `Parameters`: two `Superhuman` objects, a `hero` and a `villain`
- `Return`: one `Superhuman` object (the winner of the fight)
- The winner should be whoever has a higher strength
- The loser should reduce their strength by 1 point
- The method should print a message to the terminal saying who won and what their power was.
- The method should increase `heroPoints` or `villainPoints`, depending on who won the fight.

{{< code-action >}} **Be sure to thoroughly test `fight()` in the `main()` method.**

---


## [2] Sort the Superhumans


{{< code-action >}} **In the `main()` method, create at least 10 `Superhuman`, and add 5 to each of the arrays, `villains` and `heroes`.**


{{< code-action >}} **Add a method `sortSupers()`, that sorts the `Superhumans`.**

