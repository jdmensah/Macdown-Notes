#Load and Stress Testing 

##Definitions
###Load (capacity) Testing 
Modeling the expected usage by simulating multiple users accessing the program services concurrently 

* Will the system support the anticipated load 
* Will the system support the expected peak load 
* Is the system capable of handling increasing load over time 
* What additional resources are needed to support additional load 

Testing used to determine the stability of a given system or entity. It involves testing beyond normal operational capacity, often to a breaking point, in order to observe the results.

###Stress Testing 
Determine the stability of a given system by stressing it beyond its normal capacity
 
* Whats the maximum load until a system breaks down 
* How is the system breaking 
* Is the system able to receiver 
* When under stress, in how many ways can the system break and where ate the weak points 

###Reliability Testing 
Determine how long the application can sustain optimum performance 

###Volume Testing 

* Does the system break when handling a large volume of data 
* Is its performance affected by large volumes of data 

##Functional vs Performance Testing 
![Functional vs Performance Testing](http://cdn2.softwaretestinghelp.com/wp-content/qa/uploads/2014/01/Functional-vs-Performance-Testing.jpg)

##Load Testing - What do we need?
* Software KPIs - Key Performance Indicators 
* Expected normal load 
* Expected peak load 
* A tool to run the test 

#What could we stress test 
* number of concurrent visitors until failure 
* number of concurrent transactions until failure 
* number of pageview/sec until failure 
* unusually high number of requests to a know weakpoint 

#Load Test Tools
* HP LoadRunner 
* Jmeter 

#JMeter
* WorkBench - temporary working space
* Test plan - whole jmeter script
* thread - a single virtual 'user'
* thread group - a collection of concurrent threads 
* sampler - makes a request 
* timer - adds a delay 
* listener - reporting, logging and debugging scripts
* assertion - a checker for expected results 
* config element - configuration 
* post-processor - parses a response from the server
* pre-processor - modifies the request before sending 
* logic controllers - add logic scripts (if/else and loops)