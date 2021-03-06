# EfCore.GenericBizRunner

EfCore.GenericBizRunner (shorteded to GenericBizRunner) is a framework to help build and
run business logic when you are using [Entity Framework Core](https://docs.microsoft.com/en-us/ef/core/) for database accesses.
Its aim is to totally isolate the business logic from other parts of the application, especially the user presentation/UI layers.

EfCore.GenericBizRunner is available as a [NuGet package](https://www.nuget.org/packages/EfCore.GenericBizRunner/), 
and on the [EfCore.GenericBizRunner](https://github.com/JonPSmith/EfCore.GenericBizRunner) GitHub repo.
It is an open-source project under the MIT licence.

It provides the following features:
* A standard pattern for writing business logic, including helper classes.
* An anti-corruption layer feature that act as a barrier between the business logic and the user presentation/UI layers. 
* The *BizRunner* handles the call to EF Core's `SaveChanges`, with optional validation.
* A service, known as a *BizRunner*, that runs your business logic.
* Very good use of Dependency Injection (DI), making calls to business logic very easy.

The article [A library to run your business logic when using Entity Framework Core](http://www.thereformedprogrammer.net/a-library-to-run-your-business-logic-when-using-entity-framework-core/)
gives a good overview about the library, and there is there is 
[good documentation](https://github.com/JonPSmith/EfCore.GenericBizRunner/wiki) in the project's Wiki.
Alos, this project contains a runnable ASP.NET Core application with two business logic examples in it.

## Why did I write this library?

I have built quite a few applications that contain business logic, some of it quite complex -
things like optimisiers and pricing engines to name but a few. 
Business logic can be a real challenge, and over the years I have perfected a architecture
pattern that isolates the business logic so its easier to write and manage -
see [this article](http://www.thereformedprogrammer.net/architecture-of-business-layer-working-with-entity-framework-core-and-v6-revisited/)
and chapter 4 of my book, [Entity Framework in Action](http://bit.ly/2m8KRAZ).

Having perfected my pattern for handling business logic, then the next step was to
automate the common parts of the pattern into a library. Which is where the
EfCore.GenericBizRunner library came from.

## More information on the business logic pattern and library

The following links start with general descriptions and get deeper towards the end.
* **[This article](http://www.thereformedprogrammer.net/architecture-of-business-layer-working-with-entity-framework-core-and-v6-revisited/)**, which describes my business pattern.
* **[Chapter 4 of my book](http://bit.ly/2m8KRAZ)**, which covers building of business logic using this pattern.
* **[This article](http://www.thereformedprogrammer.net/a-library-to-run-your-business-logic-when-using-entity-framework-core/)** that describes the EfCore.GenericBizAction library with examples.
* **[Project's Wiki](https://github.com/JonPSmith/EfCore.GenericBizRunner/wiki)**, which has a quick start guide and deeper documentation.
* **[Clone this repo](https://github.com/JonPSmith/EfCore.GenericBizRunner/)**, and run the ASP.NET Core application in it to see the business logic in action.
* **Read the example code**, in this repo.  


