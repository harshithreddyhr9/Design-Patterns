# All about factory method design pattern

## Implement a factory method

We start by creating a class for our creator
* Creator itself can be concrete if it can provide a default object or it can be abstract
* Implementations will override the method and return an object

## Implementation considerations

*The creator can be a concrete class and provide a default implementation for the factory method.  
 In such cases you'll create some default object in base creator.
* You can also use the simple factory way of accepting additonal arguments to choose between different 
object types. Subclasses can then override factory method to selectively create different objects for some criteria.

## Pitfalls/Drawbacks

* More complex to implement. More classes involved and need unit testing.
* You have to start with factory method design pattern from the beginning. It's not easy to refactor existing code into factory method pattern.
* Somtimes this pattern forces you to subclas just to create appropriate instance.

## Summary

*Use factory method pattern when you want to delegate object instantiation to subclasses, you'd want to do this when you have product inheritance hierarchy and possibility to future additions to that.




