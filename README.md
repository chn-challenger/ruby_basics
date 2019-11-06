# Ruby Basics

## Objects In Ruby

Pretty much everything in ruby is an ***object*** in Ruby.  Such as:
```ruby
$ "Hello"
```
which is an example, or ***instance*** of a ```String```.
```ruby
$ 3
```
which is an example, or ***instance*** of an ```Integer```.
```ruby
$ [2,"world"]
```
which is an example, or***instance*** of an ```Array```.

Every object belongs to a type, and type is also known as ***class***.  Therefore the ***class*** of an object is the type to which it belongs to.  Almost every object you create in Ruby is an ***instance*** of some class.

## Calling Or Invoking Methods On An Object  

With any ***object*** in Ruby, depending on its ***class***, we maybe able to ***call*** or ***invoke*** some ***methods*** on that ***object***.   The ***methods*** available to call on a given object, depends on its ***class*** and are defined by its ***class***.  *Intuitively, invoking a method on an object is similar to sending a message to the object to ask it to do something.*  Once a method have been invoked on an object, you can imaging some action is performed, and at the end, something - an ***object*** is *returned*, the returned object is called the *return value* of the method.  Different methods, depending on its purpose, will obviously return different things, or objects.

When we call the ```length```method on a ```String``` instance, the method returns a ```Integer``` instance, which is the length of this string.
```ruby
$ "Hello World".length
$ => 11
```

When we call the ```odd?``` method on a ```Integer``` instance, the method returns a ```Boolean``` instance, true or false depending on if this integer is odd or not. (The ? of odd? is a part of the name of the method.)
```ruby
$ 14.odd?
$ => false
```

When we call the ```reverse``` method on a ```Array``` instance, the method returns another ```Array``` instance, based on this array, but with the elements reversed.
```ruby
$ [1,2,5,"hello"].reverse
$ => ["hello",5,2,1]
```

Methods always return some object, which does not need to be in the same class as the objects which the method was called, or invoked upon.  I.e. calling ```length``` on a ```String``` returns some ```Integer```.

## Local Variable / Object Reference / Pointer To An Object
One of the most important mechanism in Ruby, and in many languages is the setting of ***local variables***, such as
```ruby
$ my_var = "Hello world"
```
There are a few ways to understand what's happening above:
1. We set the ```String``` object ```"Hello world"``` to ***the local variable*** with the name of ```my_var```.
2. We give the ```"Hello world"``` object a ***reference name*** of ```my_var```.
3. We assign the pointer with the name of ```my_var``` to the object ```"Hello world"```.  
Interpretations 2. and 3. are the most useful, thinking of the variable name as a pointer to some ruby object which it is assigned to, or as a reference name to some ruby objects.  For example
```ruby
$ array_1 = [1,2,3]
```
Means the name ```array_1``` points to the ```Array``` instance ```[1,2,3]```, whose object id can be read by calling ```.object_id``` on the object:
```ruby
$ array_1.object_id
$ => 78980102910
```
In the code above, Firstly ```array_1``` returns the object which it is pointed to, that is ```[1,2,3]```, then calling ```.object_id``` on it.


## Mutation Methods and Non-Mutation Methods

## Ruby Docs



## Defining An Classless Method
