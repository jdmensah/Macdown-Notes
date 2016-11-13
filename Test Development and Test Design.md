#Test Development and Test Design

##Test Design 
Why do we use established test design techniques?

Because it provides us with structure, strategy and a degree of confidence from proven test designs.

--

#Context and Environment 
You must consider the context (environment) within which the task are taking place:

* The organisation 
* The maturity of the development and resting process 
* Time constraints 
* Safety or regulatory requirements
* The people involved 

--

#Test Design Specifications
A document specifying the test conditions (coverage items) for a test item, the detailed test approach and identifying the associated high-level test cases.

##Test Basis 
 
> All documents from which the requirements of a component or system can be inferred. The documentation on which test cases are based. 
  
* Functional requirements 
* technical requirements
* user requirements 

**The source of which to base the testing off**

##Test Condition
 
>An item or event of a component or system that could be verified by one or more test cases. 

**A characteristic of our software that we can check with a test**

##Test Case

>A set of values, execution preconditions, expected results and execution postconditions, developed for a particular objective or test condition, such as to exercise a particular program path or to verify compliance with a specific requirement. 

**Gets the system to some point and runs test to observe the outcome and record it**

###Test Case (Layout)

* Test Case ID  
* Precondition
* Test Data
* Expected Result	 
* Actual Result
* Pass/Fail
* Post-condition
* Comments

##Test Procedure Specification 

> A sequence of actions for the execution of a test

**All the necessary actions needed to perform the test**

###Test Procedure (Layout)

* Test Procedure Steps 
* Pass or Fail 
* Comments 

##Test Coverage 

> Provides a quantitive assessment of the extent and quality of test. 

**How much have you done**

--

#Traceability

The ability to identify related items in documentation and software, such as requirements with associated tests.

* Horizontal - through a certain level 
	*  The tracing of requirements for a test level through the layers of test documentation (e.g., test plan, test design specification, test case specification and test procedure specification or test script).
* Vertical - going through the whole level 
	* The tracing of requirement through the layers of development documentation to components

[jainbrijesh](http://www.geekinterview.com/question_details/36150) 

--

#Scheduling

Once the procedures are complete the test cases can be formed into a test execution schedule 

This defines the order in which the various test procedures are executed 
 
Test Plans must be highly dynamic due to 

* Changing Priorities
* Dependencies  
* Resources 

##Exit Criteria

The set of generic and specific conditions, agreed upon with the stakeholders for permitting a process to be officially completed. The purpose of exit criteria is to prevent a task from being considered completed when there are still outstanding parts of the task which have not been finished. Exit criteria are used to report against and to plan when to stop testing.

##Entry Criteria
The set of generic and specific conditions for permitting a process to go forward with a defined task, e.g., test phase. The purpose of entry criteria is to prevent a task from starting which would entail more (wasted) effort compared to the effort needed to remove the failed entry criteria.

##Completion Criteria 

Are explicit goals that must be attained to call an element of a project, or the entire project, "complete."

--

#Testing and Reporting 

Reporting and documenting the bugs found in the system 

[Test Plan Standards IEEE829] (http://www.fit.vutbr.cz/study/courses/ITS/public/ieee829.html) 

[Test Case Specification Template](http://www.ufjf.br/eduardo_barrere/files/2011/06/SQETestCaseSpecificationTemplate.pdf)

--

#Testing Techniques
3 Testing Techniques 

* Specification Based 
	* Based on analysis of test basis documentation, including functional and non functional without knowledge of internal structure.
* Structured Based 
	* Based on the code written
* Experienced Based 
	* Based on test cases from the tester's experience

--
 
#Specification Based - Black Box 

**Examines the functionality of an application without knowledge of its internal structures** 

* It is based entirely on the software requirements and specifications 
* Specifications can include non functional element as well as functions (reliability, usability etc)

* Sanity/smoke check 
	* not to find defects but to check health 
	* make sure the bigs reported have been fixed  


#5 Black Box Tests Page 85
* Decision Table Testing 
* State Transition Testing 
* Equivalence Partitioning
* Boundary Value Analysis
* Use Case Testing 

#Equivalence Partitioning - Black Box

In this technique, you divide the set of test condition into a partition that can be considered the same.

* Rather than trying to test infinite amounts of inputs, we strategically sample them 
* Divides a set of test conditions into partitions that can be considered the same 
* At least one value is tested from the grouped values 

Valid partition - values the system or program should accept 

Non Valid - values the system should no accept. We test these to make sure the system can handle these values 

###Advantage
* Reduces the amount of test cases we need to write

--

#Boundary Value Analysis - Black Box 

Boundary testing is the process of testing between extreme ends or boundaries between partitions' of the input values

An input value or output value which is on the edge of an equivalence partition or at the smallest incremental distance on either side of an edge, for example the minimum or maximum value of a range.

Page 90
###Boundary Value CoverageThe percentage of boundary values that have been exercised by a test suite.

Research 2 value and 3 Value analysis  

--

#Decision Table Testing - Black Box

A decision table lists all the input conditions that can occur and all the actions that can arise from them.

Decision tables are derived from business rules and conditions 

Decision table use limited entry decision tables because the number of conditions and actions can be quite large so we dont test every possible combination.

The columns in the table (business rule( represent these cases as the list both inputs and expected outputs

###Advantage
* Certain combination of conditions that are logically impossible 
* Don't forget - sometimes, we may want to test an infeasible test condition to make sure it can't run.
* Good for when input conditions have various action 

--

#State Transition Testing - Black box 

ST is concerned with systems in which outputs are triggered by changes in input state

The aim a state transition testing is:

**Finding situation where the wrong action or the wrong new state occurs** 

State - how something exist at the time 
Transitions - the change from one state to another 
Inputs or event 
Action the actions the can result from a transition 

the symbol for a state is a circle 
the symbol for a transition is and arrow 
 
**A state transition diagram is a representation of the behaviour of a system** 
 
If every valid transition is tested this is known as 0 switch coverage 

You could also test a series of transitions through more than one state 

Test cases are derived from **State Tables**

--

#Use Case Testing - Black Box

Use cases are on way of specifying functionality as business scenarios or process flow 

They capture the individual interactions between actors and the system 

Actors - ISTQB

Attrbutes of Use Cases 
there is typically a mainstrem path for 

research include & extends ISTQB 

--

#Experience Based Testing 

###Error Guessing 

A test design technique where the experience of the tester is used to anticipate what defects might be present in the component or system under test as a result of errors made, and to design tests specifically to expose them.

* Uses the testers skill and intuition and experience with similar application to the one under test
* Defect and failure lists can help identify areas that are susceptible to problems
* Fault attack approach lists possible defect and failures and design tests around that list 

##Experience Based Testing 

Testing based on the tester's experience, knowledge and intuition.

##Exploratory Testing 

An informal test design technique where the tester actively controls the design of the tests as those tests are performed and uses information gained while testing to design new and better tests.

* Five key elements 
* pridcut exploration 
* test desing 
* test executin 

Exploratory testing is done by experienced testers with an in depth knowledge of the similar system  

* Useful when specifications are missing or inadequate and there is severe time pressure 
* You still need a well defined structure rather than having a scatter gun approach 
* You also need to be able to define how complete your exploratory testing was 

**Advantages**

* Doesn't require must preparation
* Testers report a large proportion of bug via this method 

**Disadvantages**
 
* There is now review of test planning, an experienced user of the system may not be an experienced tester 
* Testers have to remember the exact steps they took to create a defect otherwise reproduction may be difficult
 
--

#Structured Based Techniques - White Box 

Used to explore system or component structures at several levels. 

* Component level - program structures 
* Integration level - exploring the way the component interact with other components
* System level - how users will interact with a menu structure 

White box test focus on ensuring that particular elements of the structure itself are correctly exercised



Tests internal structures as opposed to functional testing 

#White Box Tests
 
* Control Flow Graph 
* Simplified Control Flow Graphs
* Statement Testing and Coverage 
* Decision Testing and Coverage 


Pseudcocde - detailed yet readible description of whst a computer program or couter algorithm must due expressign a 

#Control Flow Graph - White Box 

**Provide a method of representing the decision points and the flow of control within a piece of code**

Like a flow chart but only shows the decisions 

![What the graph is made up of](http://www.softwaretestinggenius.com/photos/ISBF54A.JPG)

![Control flow graph](http://www.softwaretestinggenius.com/photos/ISBF55A.JPG)

#Statement Testing and Coverage - white box

Technique aimed at exercising programming statements 

If we aim to test every executable statement we call this **100% statement coverage**  
If we to test of of the executable statements we call this **50% statement coverage**

**We are only interested in executable statements**
**We do not count non-executable statements when measuring coverage**

#Decision Testing and Coverage - White Box

* Ensure that the decision in a program are exercised 
* To test a decision we need to exercise it when the associated condition is true and when the condition is false 
* This guarantees that both exit from the decision are exercised
* Coverage is measured by counting the number of decisions executed divided by the total number of decision outcomes in the program 

100% branch coverage implies 100% decision coverage 

#Simplified Control Flow Graphs - White Box 

They incorporate less detail since their purpose is to identify control structures but not the detail of code

 