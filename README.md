# reimagined-design-patterns

Give a summary description of Four design patterns that you choose from the following design patterns: **Adapter,  Builder, Composite, Decorator, Observer, Interpreter, State, Mediator, Memento, Prototype, Proxy**. In your summaries say:

- what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example
- how the pattern works, what the basic idea of the pattern is
- what the main advantage and what the the main disadvantage is of using this pattern
- Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more). 

> Do not add diagrams, and do not try to give a complete description of the patterns as found in the books. Rather think of how you would explain the essential ideas of these patterns in a few sentences to a colleague while drinking coffee.



**1. Adapter**

**Summary:**

One interface of class to any other interface. Requester can see only the target class. Adapter implements target class and takes all request to different interface which is going to adapt for the requirement.

**what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example**

It solves the problem of two different interfaces communicating each other directly.
For example: Consider Fish as an interface has the behavior (swim) and Athlete as another interface has behaviors like (run, speak). In order to make a swimming athlete who can have all the behaviors (swim, run, speak) we can create a SwimmerAdapter which implements Fish and inside the instance of Athlete been created. Hence we will finally get all three behaviors from SwimmerAdapter by combining two different interfaces to give it to swimming athlete.

**Basic idea of the pattern:**

Basic idea is to bind two different irrelevant interface to provide a combined class implementation.

**Advantage:**
Can reuse the existing interface functionality to our end class features.

**Disadvantage:** 
Code will look quite strange while different irrelevant interface implemented on meeting one requirement.


**2. Observer**

**Summary:** 

Observable is an object which notifies observers about the changes in its actions. Observable act as a publisher and gives the updates to all observers who acts as a subscribers,

**what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example**

when publisher gave new updates observable need to change it state, hence observer will listen to the change and accepts it. For example: IoT enabled two wheeler system built to get notification updates of speed information to our mobile phones. The Speedometer details need to be send by a publisher mechanism and clients mobile phones act as subscribers will be listening to the updates.

**Basic idea of the pattern:**

Mechanism when one publisher need to notify all its subscribers to get the updates.

**Advantage:**
Instant communication and immediately all observers getting information at the same time.

**Disadvantage:**
Unknown observers also can come into picture which results in leakage of information.


**3. Proxy**

**Summary:** 

Proxy design pattern works like a shadow to get the functionality of the real object. 

**what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example**

In case of immediate action to be taken by an object which is not available that time, a proxy of that instance will do the necessary function. For example: When you want to pay for the purchase you made on a shopping mall, we can use the proxy of direct money to digital money with the help of Gpay,paytm etc, which act as a proxy here.

**Basic idea of the pattern:**

Idea is to make use of shadow instance instead of direct instance at sometimes.

**Advantage:**
Major advantage of using proxy is to avoid creating duplicate instances and perfect memory utilization.

**Disadvantage:** 
This pattern sometimes introduce different levels of data hiding which results in lack of information to main object.


**4. Prototype**

**Summary:** 

Prototype pattern allows us to create a copy of existing object when a new instance creation takes time to create. This reduce time of creation of new instances and memory allocation in much better way. For example: When a bulk of movie data has same informations like title, language, genre, to store in the database we need not to create each instance everytime, we can create one instance and do a copy instance and iterate and store all the records. This saves memory and time of new instance creations.

**Basic idea of the pattern:**

Idea of creating copy instance instead of creating new instance to save time and memory.

**Advantage:**
Reduce new object creations and memory optimization when a new object is quite costly. Hence using existing object is clone to achieve the result.

**Disadvantage:** 
The main disadvantage of using this pattern is all the child class need to utilize this cloning functionality which is not followed in traditional design.