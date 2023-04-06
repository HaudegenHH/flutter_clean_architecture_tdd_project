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
