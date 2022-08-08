# Unity 3.4

https://unity3d.com/unity/whats-new/unity-3.4

## JavaScript upgrade guide



*   Unity 3.4 ships with an improved javascript compiler that supports better type inference heuristics for commonly used Unity APIs such as [GameObject.GetComponent](http://docs.unity3d.com/Documentation/ScriptReference/GameObject.GetComponent.html) and [Object.Instantiate](http://docs.unity3d.com/Documentation/ScriptReference/Object.Instantiate.html) as well as a stricter strict compilation mode (#pragma strict). The benefits are improved error checking and more efficient code generation leading to faster execution times. The downside is that in some particular cases code that compiles cleanly with Unity 3.3 might be (correctly) refused by the 3.4 compiler as in the following example:
    
    // var definition in Foo.js private var value = 42;
    
    // attempt to use Foo.value in Bar.js GetComponent(Foo).value = 21;
    

#### In Unity 3.3 the code above compiles without errors but 3.4 will complain with something similar to: