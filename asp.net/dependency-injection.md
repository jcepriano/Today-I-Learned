### Dependency Injection in an ASP.NET Core App

Dependency Injection at a high level is the action of injecting an external component into a class rather than the class
creating the component itself. If I was trying to use a database in a class, I could inject that database by adding it as an argument to 
the constructor. Rather than creating a new database object.

### Advantages
One of the biggest benefits of Dependency Injection was that it allows for class coupling to be reduced. To reduce class coupling is to
minimize the degree of interdependence or the connections between different classes.

### Disadvantages
One drawback is that the code can be very complex because of the dependencies being defined and managed explicitly. 
Dependency injection can also result in a larger number of classes in the program.

Initializing Database
```
public ShoppingCart()
    {
        _database = new Database();
    }
```
Injecting Database
```
public ShoppingCart(Database database)
    {
        _database = database;
    }
```

Resources:

https://devopedia.org/dependency-injection#:~:text=Dependency%20Injection%20is%20considered%20a,part%20of%20SOLID%20Design%20Principles.

https://www.techtarget.com/searchapparchitecture/definition/dependency-injection

https://www.tutorialsteacher.com/ioc/dependency-injection

https://sourcemaking.com/design_patterns
