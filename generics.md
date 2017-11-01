<!-- What is one benefit of using generics in Java classes? -->
They allow you to instantiate a class with a different property type.
E.g. Allowing you to use the same class to give an id_number as both a string and an int.

<!-- Name an example of a generic class that we have used in Java?
 <!--  -->
ArrayList<Card> cards = new ArrayList<Card>();

<!-- What is the syntax for declaring a generic class? -->
1. public class Class<T>{

2. private T object;

3. public Object(T object)
}


<!-- At what point does the generic type get specified? -->
In the class declaration i.e. line 2 in the answer above.



<!-- Can generic types be of primitive type? -->
No, to maintain compatibility with previous versions of Java (https://stackoverflow.com/questions/2721546/why-dont-java-generics-support-primitive-types)

Can a generic class take more than one type parameters?

Yes: you can declare multiple parameters on a generic class.
e.g. public <S, T> void func(Set<S> s, Set<T> t) https://stackoverflow.com/questions/1759549/java-generics-multiple-generic-parameters
