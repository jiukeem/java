// -------------------------------------- lesson1. hello world! --------------------------------------

public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
// think 'class' as a single concept in java
// 'main' is a method which the program tasks
// String[] args is a placeholder for information we want to pass into our program.
// for multi-line comment, use /* */
// Java does not interpret whitespace.
// Java does interpret semicolons. Semicolons are used to mark the end of a statement, one line of code that performs a single task.
// There are no semicolons at the end of a curly brace. No semicolons for classes or methods!


// -------------------------------------- lesson2. Variables --------------------------------------

// primitive data types are int, double, boolean, char: they do not have built-in behavior
// String is object data type and has built-in behavior.
// String uses "" and char uses ''
// Static typing, which is one of the safety features of Java. -> catch error while compiling not execution(runtime error)


// -------------------------------------- lesson3. Manipulating Variables --------------------------------------

// -------------------------------------- lesson4. Introduction to Classes --------------------------------------
public class Store {
    // instance fields
    String productType;
    int inventoryCount;
    double inventoryPrice;

    // constructor method
    public Store(String product, int count, double price) {
        productType = product;
        inventoryCount = count;
        inventoryPrice = price;
    }

    // main method
    public static void main(String[] args) {
        Store lemonadeStand = new Store("lemonade", 42, .99);
        Store cookieShop = new Store("cookies", 12, 3.75);

        System.out.println("Our first shop sells " + lemonadeStand.productType + " at " + lemonadeStand.inventoryPrice + " per unit.");

        System.out.println("Our second shop has " + cookieShop.inventoryCount + " units remaining.");
    }
}
// A class is the set of instructions that describe how an instance can behave and what information it contains.
// public is an access level modifier that allows other classes to interact with this class.
// main() runs when we compile file.
// We create objects (instances of a class) using a constructor method. The constructor is defined within the class.
// 'within' the class! different from python
public class Car {
    public Car() {
        //constructor method starts after curly brace

        //instructions for creating a Car instance

    }
    //constructor method ends after curly brace

    public static void main(String[] args) {

        // program tasks

    }
}
// Car() itself is a contructor(shares name with class)
// We create instances by calling or invoking the constructor within main().
public class Car {

    public Car() {
    }

    public static void main(String[] args) {
    /*
    invoke a constructor using
    'new', the name, and parentheses:
    new Car()
    */
        Car ferrari = new Car();
    }
}
// type instance in main method not constructor!
// the first Car is data type of this variable(instance). Just like String!
/*
Review the order of the printed messages:

Running the program invokes main()
We create an instance so we move from main() to Store()
The code inside Store() runs
When Store() finishes execution, we return to main()
 */

public class Car {
    // instance fields
    String color;

    // constructor method with a parameter
    public Car(String carColor) {
        // parameter value assigned to the field
        color = carColor;
    }

    // main method
    public static void main(String[] args) {
        // program tasks
    }
}
// we need to add parameter for value of the instance field. These values become the state of the instance.
// Classes define the state and behavior of their instances.
// Behavior comes from methods defined in the class.
// State comes from instance fields declared inside the class.

public class Dog {
    // instance field
    String breed;
    // constructor method
    public Dog(String dogBreed) {
    /*
    value of parameter dogBreed
    assigned to instance field breed
    */
        breed = dogBreed;
    }
    public static void main(String[] args) {
    /*
    create instance:
    use 'new' operator and invoke constructor
    */
        Dog fido = new Dog("poodle");
    /*
    fields are accessed using:
    the instance name, `.` operator, and the field name.
    */
        fido.breed;
        // "poodle"
    }
}


// -------------------------------------- lesson5. Methods --------------------------------------

// public means that other classes can access this method. We will learn more about that later in the course.
// The void keyword means that there is no specific output from the method.
public class Store {
    // instance fields
    String productType;
    double price;

    // constructor method
    public Store(String product, double initialPrice) {
        productType = product;
        price = initialPrice;
    }

    // increase price method
    public void increasePrice(double priceToAdd){
        double newPrice = price + priceToAdd;
        price = newPrice;
    }

    // get price with tax method
    public double getPriceWithTax(){
        double tax = 0.08;
        double totalPrice = price + price*tax;
        return totalPrice;
    }

    public String toString() {
        return "This store sells " + productType + " at a price of " + price + ".";
    }

    // main method
    public static void main(String[] args) {
        Store lemonadeStand = new Store("Lemonade", 3.75);
        Store cookieShop = new Store("Cookies", 5);
        System.out.println(lemonadeStand);
        System.out.println(cookieShop);

    }
}
/*
Defining a method : Methods have a method signature that declares their return type, name, and parameters
Calling a method : Methods are invoked with a . and ()
Parameters : Inputs to the method and their types are declared in parentheses in the method signature
Changing Instance Fields : Methods can be used to change the value of an instance field
Scope : Variables only exist within the domain that they are created in
Return : The type of the variables that are output are declared in the method signature
 */


// -------------------------------------- lesson6. Conditionals and Control Flow --------------------------------------
if (condition) {
    // consequent path
} else {
    // alternative path
}


// -------------------------------------- lesson7. Conditional Operators --------------------------------------

// -------------------------------------- lesson8. Arrays --------------------------------------
// An array holds a fixed number of values of one type.
// 'fixed' number, 'one' type -> different from python
// when you print array, you get the address of array not the content.
// If we want to have a more descriptive printout of the array itself, we need a toString() method that is provided by the Arrays package in Java.
// Empty arrays have to be initialized with a fixed size.
String[] menuItems = new String[5];
// Once you declare this size, it cannot be changed.
// We can also change an item after it has been assigned. but it should be same data type.

public class HelloYou {
    public static void main(String[] args) {
        System.out.println("Hello " + args[0]);
    }
}
/*
In this case, the array args contains the arguments that we pass in from the terminal when we run the class file.
(So far, args has been empty.)
When we run the file HelloYou in the terminal with an argument of "Laura":
java HelloYou Laura
We get the output:
Hello Laura
 */
import java.util.Arrays;

public class Newsfeed {

    String[] topics;

    public Newsfeed(String[] initialTopics) {
        topics = initialTopics;
    }

    public static void main(String[] args) {
        Newsfeed feed;
        if (args[0].equals("Human")) {

            //topics for a Human feed:
            String[] humanTopics = {"Politics", "Science", "Sports", "Love"};
            feed = new Newsfeed(humanTopics);

        } else if(args[0].equals("Robot")) {

            //topics for a Robot feed:
            String[] robotTopics = {"Oil", "Parts", "Algorithms", "Love"};
            feed = new Newsfeed(robotTopics);

        } else {
            String[] genericTopics = {"Opinion", "Tech", "Science", "Health"};
            feed = new Newsfeed(genericTopics);
        }

        System.out.println("The topics in this feed are:");
        System.out.println(Arrays.toString(feed.topics));
    }
}
// you can select task according to input
/*
Creating arrays explicitly, using { and }.
Accessing an index of an array using [ and ].
Creating empty arrays of a certain size, and filling the indices one by one.
Getting the length of an array using length.
Using the argument array args that is passed into the main() method of a class.
 */


// -------------------------------------- lesson9. ArrayLists --------------------------------------

// arraylist is dynamic array!
/*
Store elements of the same type (just like arrays)
Access elements by index (just like arrays)
Add elements
Remove elements
 */
// We use angle brackets < and > to declare the type of the ArrayList.
// These symbols are used for generics.
// Generics are a Java construct that allows us to define classes and objects as parameters of an ArrayList.

// This code won't compile:
ArrayList<int> ages;

// This code will compile:
ArrayList<Integer> ages;

// The <Integer> generic has to be used in an ArrayList instead.
// You can also use <Double> and <Char> for types you would normally declare as doubles or chars.
// Declaring:
ArrayList<Integer> ages;
// Initializing:
ages = new ArrayList<Integer>();
// Declaring and initializing in one line:
ArrayList<String> babyNames = new ArrayList<String>();

/*
Adding a new ArrayList item using add(value).
Accessing the size of an ArrayList using size().
Finding an item by index using get(index).
Changing the value of an ArrayList item using set(index, value).
Removing an item with a specific value using remove(index or value).
Retrieving the index of an item with a specific value using indexOf(value).
 */