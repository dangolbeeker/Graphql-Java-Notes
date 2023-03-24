 
 
 Google Guice notes 
 
 ## 
 
 Guice creates and provides a single instance of that class throughout the application. This instance is typically thread-safe, 
 as Guice synchronizes access to the instance to ensure that it is not modified concurrently
 @Singleton or asEagerSingleton()
 
 `asEagerSingleton()` method, the singleton is created eagerly when the injector is first created, which can improve startup times.
 
 `asEagerSingleton()` is a method in Google Guice that allows you to eagerly initialize a singleton-scoped binding upon creation of the injector . This means that the singleton instance will be created as soon as the injector is created, rather than waiting until it is first accessed.

Using asEagerSingleton() can be useful in cases where you want to ensure that the singleton is fully initialized and ready to use before any other part of the application is started. It can also potentially improve the startup time of your application,
 since the singleton instance will already be initialized when it is first accessed.
 
 
 
 
 
 AbstractModule is a helper class used to add bindings to the Guice injector in the Google Guice library for dependency injection in Java .
 When a class extends AbstractModule, it becomes a module that can define one or more bindings between a service interface and its implementation. 
 The bindings can specify the scope of the service implementation, such as Singleton or RequestScoped.