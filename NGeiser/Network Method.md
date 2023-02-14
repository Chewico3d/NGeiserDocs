# Network Method
This page shows how to create a Network Method in NGeyser, these classes will be saved in InternalCaller

## Structure
To declare a static funtion you just need to create a funtion that contains [NetworkParameters](/) as the function parameter \
Then the internal caller stores the method with the name : ClassName.MethodName

```cs
using NGeyser;

//This class is derived from NetworkClass to allow store the NetworkMethods
class ExampleClass : NetworkClass {
    //In this example geyser will sorage the method
    //with the id : "ExampleClass.MethodName"
    void MethodName(NetworkParameters parameters) {
        //Do stuff
        Console.WriteLine("I have recived a message!!!");
    }
}
```