## Flutter, Clean Architecture & TDD

### Useful link:

Blog about "Uncle Bobs" - "The Clean Architecture"

https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html

### Important!

Since Dart 3 introduced null-safety, there are several dependency problems so just run the tests without it.

Therefore go to:

Preferences -> Settings -> User Settings ->and search for:


> flutter test additional args


Add Item:
```sh 
--no-sound-null-safety
```


---

code refactoring: 

like in php you can make use of the call method, which is an inbuild fn and allows you to call the obj as if it were a method.
therefore you can get rid of the execute and replace it with call

next:

wrote an abstract class (since dart doesnt support interfaces) that enforces the class "GetConcreteNumberTrivia" to have a call method (and not an execute method like before)
and i put it into the core/usecases folder. it applies to all the usecases across all of the features thats y i put it into the core folder
