## Explain java flame

Stack capturing  
Arguments parsing  
Json output  

## Show javaflame working

Execute once capturing all and show flamegraph  
Show search by term  
Click on some entry and show data  
Change argument to capture only one Class  
Change argument to capture only one Class Function  
Change argument to capture two classe with regex  

## Explain Java Instrumentation API

Introduced with java 1.5
Instrumentation is the addition of byte-codes to methods for the purpose of gathering data to be utilized by tools.
Redefine (give new byte code, respecting signatures and inheritance) and Retransform (manipulate byte code)
Show premain.
A java agent is a regular java progam called at the jvm initialization (also after initialization form jvm 1.6 onwards).
The transformer is called when classes are loaded, when they are redefined. and if canRetransform is true, when they are retransformed.
Called berfore Main.

## Show java agent that changes a sum

...

## Explain what profilers do

## Profilers
Profilers sample the call stack trace periodically.  
Cheap, fast unintrusive.  
No extra state is kept in memory.  
Interested on how long it takes for method calls.  

## Javaflame
Javaflame instruments every call.  
Expensive and intrusive.  
Keeps a separate stack in memory.  
Calls toString on parameters.  
Writes to a file periodically.  
Interested in what calls what and the values.  
Also allows code interception.  
