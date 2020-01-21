# Defining and Instantiating Classes

If you are familiar with creating and instantiating classes in Java at a fundamental level, you know that if you've written a java file and compiled it, you've created a class by doing  
```java
public class Hello{
	public static void main (String[] args) { ..  }
}
```

## Separate compilation 

Since this is a review of Java and I'm not learning Java, I don't have to act surprised knowing that not all classes will have a main method.  
For example:  
```java
// Dog.java

public class Dog {
	public static void makeNoise() {
		System.out.println("Bark!");
	}
}
```

The code above will compile if you do `javac Dog.java` BUT it will not run if you type `java Dog`, because there is no main method.

It's often the case that classes created will not actually have a main method, instead you would create a driver class with a main method.  
The driver will then instantiate your classes and call whatever methods it needs to on those objects.

`DogDriver.java` for will call the static method `makeNoise` in `Dog.java`

