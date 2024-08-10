# Counter MVC

This project is for learn how to implement MVC in C.

In the diagram We could see there are two services.
The first I call counter. Very original!!
The second I call display. 

Both will communicate between UDP protocol. 

Counter is the domain. Very simple. 
We have the controller where will get the counter and convert to DTO Output
And finally will encode in JSON to send through network

THe display will receive the message in JSON.
deserialize the JSON and generate the Input DTO
Convert into Counter Domain and Store in repository.
All these coordinations will be made by controller
With the data in the repository
Presenter will read and convert the counter in Representation
and put on the view which is just a printf 



Let's go...

These are the basic structure.
First we start from counter. I'll paint the blocks with colors when I finish the 
implementation.

Inside the controller folder I have two more folders, the data_provider and the dto
inside dto folder We can create the counter output. It will convert the counter domain into counter output.


Here I'll choose the value pass to force be constant

Now we can create the provider which will convert the dto into JSON.

I finished the provider. Now let's join all together with controller

sat scheduler needs an event.


And we are receiving the data.