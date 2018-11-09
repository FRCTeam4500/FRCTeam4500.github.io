# Variables
For the scope of programming the robot, the following are the most important variables.

| Variable | Description                                                                               |
|----------|-------------------------------------------------------------------------------------------|
| int      | Can be used to represent any Integer number. Examples are 0, 7, -16, 1253.                | 
| double   | Can be used to represent decimal values. Examples are 1.2, -643.1742, 3.14159             |
| boolean  | Can be used to represent true or false                                                    |
| String   | Can be used to represent a sequence of text. Examples are "Hello, world", "2 plus 1 is 3" |

For a complete list, visit [Oracle's website](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html)

```java
int myVar;
myVar = 2;

int numOne = -5;
double PI = 3.14159;
boolean isRaining = false;
String username = "ch1ckenS1ayer123";
```

# Operators
| Operator    | Use                                                           |
|----------   |---------------------------------------------------------------|
| > and >=    | Greater than and greater than or equal to                     |
| < and <=    | Less than and less than or equal to                           |
| =           | Assignment. Used for setting variables                        |
| ==          | Checks if two variables are equal to each other               |
| !=          | Checks if two variables are not equal to each other           |
| +           | Adds two variables                                            |
| -           | Subtracts two variables                                       |
| *           | Multiplies two variables                                      |
| /           | Divides two variables                                         |
| %           | Mod operator. Finds the remainder (11 % 3 = 2)                |
| ++          | Increment. Increases a variable by one (varName++)            |
| --          | Decriment. Decreases a variable by one                        |
| +=, /=, etc | Applys the operation and updates the variable. (varName += 2) |

For more information, view: [arithmetic operators](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/op1.html) and [equality operators](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/op2.html)
# If statements

```java
boolean isRaining = false;
boolean isCold = true;

if(isRaining == true && isCold == false) {
    System.out.println("It's raining. Bring an umbrella!");
} else if(isRaining == true && isCold == true) {
    System.out.println("It's snowing!");
} else {
    System.out.println("It's not raining");
}
```

```java
int temperature = 32;
boolean willFreeze = false;
boolean willBoil = false;

if(temperature < 32) {
    willFreeze = true;
} else if (temperature == 32) {
    System.out.println("You are at the freezing point!");
} else if(temperature > 32 && temperature < 212) {
    System.out.println("It's your every day boring temperature");
} else if (temperature >= 212) {
    willBoil = true;
} else if (temperature != 5) {
    System.out.println("The temperature is not 5");
} else {
    System.out.println("Nothing interesting here");
}
```

# For loops

```java

// for(variable to count with; when to stop; by how much the variable should be changed)

// Prints the numbers 0 through 9
for(int i = 0; i < 10; i++) {
    System.out.println(i);
}

// Prints the numbers 0 through 9 backwards
for(int i = 9; i >= 0; i--) {
    System.out.println(i);
}

// Prints even numbers up to 20
for(int i = 0; i <= 20; i+=2) {
    system.out.println(i);
}

// Prints (0, 0), (0, 1), (0, 2), (1, 0), (1, 1), etc
for(int x = 0; x < 3; x++) {
    for(int y = 0; y < 3; y++) {
        System.out.println("(" + x + "," + y + ")");
    }
}
```