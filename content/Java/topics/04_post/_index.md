---
title: "Posts" 
bookFlatSection: false
weight: 6
# bookCollapseSection: true
draft: true
---

# Posts
This lab uses Java OOP principles. It emphasizes using class objects inside other classes.

---

## [0] Setup


### Clone the Repository

#### 💻 select [`Projects`] > [`Get from VCS`] > [`Repository URL`]

{{< figure src="images/courses/java/intellijIDEA/intellij_repo_url.png" width="50%">}}


 
{{< code-action "Paste your URL to clone the lab">}} 

Be sure to change `yourgithubusername` to your actual GitHub username.

```shell
https://github.com/isf-dp-cs/lab_cards_yourgithubusername
```

---

## [1] Cards

The class Cards has already been written for you. It is a simplified version of the Cards you wrote last class. 

{{< mermaid >}}

classDiagram
    class Post {
		- textContent: String
        - hashtag: String 
    	- likes: int 
        - visibility: boolean
        + default constructor()
        + accessors and mutator methods  ()
    }

{{< /mermaid >}}

{{< mermaid >}}

classDiagram
    class Profile {
		- username: String
        - firstName: String 
    	- age: int 
        - myPosts: Post[]
        + Profile(String username, String firstName, int age)
        + sortPosts() void
        + accessors and mutator methods  ()
    }

{{< /mermaid >}}


{{< columns >}}
```java
public class Student {
	// attributes 
    private String name;
    private String[] subjects;

	//constructor
    public Student(String name, String[] subjects) {
        this.name = name;
        this.subjects = subjects;
    }

	//accessors and mutators
    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public String[] getSubjects() {
        return subjects;
    }

    public void setSubjects(String[] subjects) {
        this.subjects = subjects;
    }
}
```

<--->

{{< mermaid >}}
classDiagram
    class Student {
		-String name
    	-String[] subjects
		+Student(String name, String[] subjects)
        + getName(): String
        + setName(name: String): void
        + getSubjects(): String[]
        + setSubjects(subjects: String[]): void
    }
{{< /mermaid >}}

{{< /columns >}}

There are a few main differences:

### Only 2 attributes

```java
public class Card {
    private String suit;
    private int rank;
```

### Overriding toString()

This method overrides `toString()`. This means that now, if you use `System.out.println()` on a `Card` object, it will print nicely to the console:

```java
   // Override toString
    // Converts the card to a readable string representation.
    @Override
    public String toString() {
        String rankString;
        if (rank >= 2 && rank <= 10) {
            rankString = String.valueOf(rank);
        } else if (rank == 11) {
            rankString = "Jack";
        } else if (rank == 12) {
            rankString = "Queen";
        } else if (rank == 13) {
            rankString = "King";
        } else if (rank == 1) {
            rankString = "Ace";
        } else {
            rankString = "Invalid Rank";
        }
        return rankString + " of " + suit;
    }
```

---

## [2] Deck

The `Deck` class uses the `Card` class to make a deck of cards. It will store all the cards into an array.

{{< mermaid >}}
classDiagram
    class Deck {
		-Card[] cards;
    	-int topCardIndex;
        + Deck()
        + shuffle(): void
        + dealCard(suit: String): Card
    }
{{< /mermaid >}}

It is your job to finish the Deck class according to the specifications.

---

### Deck Constructor

💻 **Complete the  constructor so it does 2 things:**

#### 1️⃣ initialize `topCardIndex` to its starting value of 0
> *The `topCardIndex` keeps track of which card is the current "top card".*

#### 2️⃣ initialize `cards` with all 52 cards from the deck

>To create all the cards in a deck, you can use nested for-loops to combine the 4 possible suit (❤️♠️♦️♣️) with the 13 possible ranks (1,2,3,4,5,6,7,8,9,10,11,12,13)
>
>Here is an example of using nested `for loops` to generate all possible weekday blocks:
```java
String[] days = {"Monday", "Tuesday", "Wednesday", "Thursday", "Friday"};
int[] blocks = {1, 2, 3, 4, 5};

for (int i = 0; i < days.length; i++) {
    for (int j = 0; j < blocks.length; j++) {
        System.out.println(days[i] + " block " + blocks[j]);
    }
}
```

---

### shuffle()

💻 **Write a method `shuffle()` that randomly swaps the `card` objects inside the `cards` array**

1️⃣ loop through every position `cards` array   
2️⃣ each time you loop, randomly generate another location in the array, `rand_i`     
3️⃣ swap the `card` located at `i` with the `card` located at `rand_i`    

> Here's how to randomly generate a number 0-10:   
```java
Random rand = new Random(); // you only need to run this once
int randomIndex = rand.nextInt(10); //each time you need a new random number, run this line of code
```


---

### dealCard()
💻 **Write a method `dealCard()` that returns the next `card` in the deck**

1️⃣ if the `topCardIndex` isn't null, return the card there, then increase `topCardIndex` by 1   
2️⃣ else, return `null`

---

## [3] Java Arrays


Here are some examples of how to use Java arrays:

### **Making a Array with Values**
```java
// Create an array of 5 int elements
int[] marks = {10, 20, 30, 40, 50};
```

### **Making a Array without values, then adding them**
```java
int[] marks = new int[3];
marks[0] = 50; 
marks[1] = 70;
marks[2] = 93;
```

### **Changing an Element Value**
```java
int[] nums = {1, 2, 0, 4};
// Change value at index 2
nums[2] = 3;
```

### **Get the length of an array**
```java
marks.length
```

---

## [4] Deliverables

{{< deliverables>}}


### Push to Github

{{< code-action "Select Commit from the menu on the left." >}} Select all your updated files. **Be sure to include a descriptive commit message.**

{{< figure src="images/courses/java/git_commit_1.png" width="40%">}}
{{< code-action "Click Commit and Push" >}} 

{{< figure src="images/courses/java/git_commit_2.png" width="40%">}}

{{< code-action "Click Push" >}}  
{{< figure src="images/courses/java/git_commit_3.png" width="40%">}}



{{< /deliverables>}}
