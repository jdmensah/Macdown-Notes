#Software Testing 
[ISTQB Glossary] (http://astqb.org/glossary/)

##Fundamentals of Testing

###What is Software Testing 
Software testing is a process of executing a program or application with the intent of finding the software bugs. It can also be stated as the process of validating and verifying that a software program or application or product: Meets the business and technical requirements that guided it's design and development.

Tester/Developer Mindset  
Quality Assurance  
Risk & Quality - testing allow us to mitigate risk   
Risk - a factor that could result in future negative consequences, usually expressed as **impact and likelihood**

The effect of testing is to give an indication of the software quality

##Seven Testing Principles

1. **Testing shows the presence of bugs** 
	* Testing to find bug in the system
2. 	**exhaustive testing is impossible **
	* impossible to test every aspect of the system for bugs 
3. **early testing**
	* Testing the product early to catch bugs and correct any issues. Ensure quality from the start
4. **defect clustering**  
	* When a small number of modules/units contains most of the bugs detected or show the most operational failures.
		* This can occur because of:
		* System complexity 
		* volatile code 
		* development staff experience/inexperience 
5. **the pesticide paradox**
	* If the same tests are repeated over and over again, eventually the same test cases will no longer find new bugs.
6. **testing is context dependant**
	* The same test you run a system may not apply to another aspect of it
7. **absence of errors fallacy**
	* Just because the software shows no errors doesn't necessarily mean it is ready to be shipped

###Key Testing Terms
* **Defect** - A flaw in a component or system that can cause the component or system to fail to perform its required function
* **Root cause vs effect**
	- treating the symptoms and not the cure
	- solving the root of the problem and not just fixing the issue
* **Error** - A human action that produces an incorrect result. 
* **Failure** - Deviation of the component or system from its expected delivery, service or result.
* **Fault** 
* **Mistake** - A human action that produces an incorrect result.
* **Bug** - a bug is a error the decreases the value of the product.

[Bugs and Defects] (http://istqbexamcertification.com/what-is-defect-or-bugs-or-faults-in-software-testing/)

###Debugging and Testing 
Debugging - used by developers to identify the cause of bugs or defects in code and undertake corrections

Testing - systematic exploration of a component or system with the main aim of finding and reporting defects 

--
#Fundamental Test Process 
###Testing lifecycle 

![Fundamental Test Process] (http://cf.ppt-online.org/files/slide/m/mnUMay2k16dt40vzLpPYfiCbBgGZ7TIsJE8Q5F/slide-25.jpg)

* Planning & Control 
* Analysis & Design 
* Implementation & Execution
* Exit Criteria & Reporting 
* Closure Activities 

**Planning & Control**  
Determine what is going to be tested  
How it is going to be tested  
Who will do the testing  
Define exit criteria   
Monitoring and control feedback into the continual   Activity of planning   

**Analysis & Design**  
Reviewing the test basis   
Identify test conditions cases and procedures   
Design the tests  
Detail the test environment and tooling   
Highlight the test data   
Create traceability between test basis and test cases   

**Implementation & Execution**  
Prioritising test cases, creating test data and writing test procedures  
Creating test suites from collected test cases - Consists of test automation scripts.  
Checking environment is set-up correctly  
Running tests in determine order  
Log testing activities and defects   
Reporting incidents

**Exit Criteria & Reporting**  
Ensure the criteria been met to satisfy the stake holder   
Determine if more tests need to be made  
Checking the system is in a ready state for release  
Writing up results for sponsors and stakeholders 

**Test Close Activities**   
Making sure everything is tidied away  
Ensure documentation is in order  
Closing down and archiving the test environment 

#Order of Importance  
Below are people who could test software, listed in order of increasing importance 

1. Those who wrote the code 
2. Members of the same development team 
3. Members of a different group (independent test team)
4. Members of a different company (a testing consultancy/outsourced)

--

#Development Models 

**Testing is Context Dependant**

* The nature of the project 
* The project schedule
* The resources available  

--

#Verification vs Validation 
###Verification 
Checks the work-product meets the requirements set out

* Current
* No ambiguity
* No errors 

**Verification ensure that we are building the product the right way**

###Validation
Checks the work-product against the users needs 
 
* Evaluation against user needs rather than work-product  
* Ensure behaviour of the product meets customer needs   
* Helps to make sure we are building the right product for our users

**Validation ensures we are building the right product for the user**

--

#Software Testing Models 
* **Waterfall**
* **V Model** 
* **Iterative and Incremental**

--

#Waterfall Model
![Waterfall Model](http://www.softwaretestinggenius.com/photos/ISBF2.JPG)
 
Requirements Specification  
Functional Specification   
Technical Specification  
Program Specification   
Coding   
Test

Each work-product or activity is completed before moving on to the next  

At every stage there should be a check to see if the work product meets its objectives. Once it passes that check we can progress to the next stage of development

###Advantage
* Good for projects that follow a specific set of procedures 
* Good for projects where the requirements are unlikely to change

###Disadvantage 
* Quality is not assured throughout the lifecycle

--

#The V-Model
![V-Model] (http://3.bp.blogspot.com/-FbypDlBKlFQ/Tdp5NPRSwII/AAAAAAAAACQ/U5QZzAzwKF4/s1600/V%2BModel.jpg)

**Left hand side focuses on the gathering requirements**

These are the work products

* **Requirements Specification** - Capturing of user needs. 
* **Functional Specification** - definition of functions required to meet user needs. 
* **Technical Specification** - technical design of functions identified in the functional specification
* **Program Specification** - detailed design of each module or unit to be built to me required functionality 

**Right hand side focuses on test activities**

These are the activities

* Testing against the **requirements specification** take place at the *acceptance testing* stage
* Testing against the **functional specification** take place at the *system testing* stage 
* Test against the **technical specification** takes place at the *integration testing* stage 
* Testing against the **program specification** takes place at the *unit testing* stage

###Advantages
* defects can be identified early as possible 
* Integrates testing into the whole dev process
* test are based on what the system should do no what it does

###Disadvantages
* Less documentation
* If user requirements are not captured correctly these issues can effect final product

--

#Iterative Models
![Iterative Model](http://www.softwaretestinggenius.com/photos/ISBF5B7.JPG)

Requirements do not need to be fully defined before coding can begin 

Time-boxing is used to define timescale

###Advantage
* Working version of the product are built, in stages (iterations) 
* Users are involved in the testing - reduces risk of developing wrong product 
###Disadvantage 
* Lack of formal documentation
* developers make changes without formally recording them - changes cannot be tracked back to requirements 
* large amount of regression testing 

--

#Test Levels

The test level provides and indication of the focus of the testing 

**Unit (Component) Testing**
**Integration testing** 
**System testing** 
**Acceptance Test** 

--

#Test Driven Development 
![](https://www.perforce.com/sites/default/files/images/tdd.png)

--

#Unit Testing
Testing section of the system for functionality 

* Units are also called programs, modules or components 
* Code is usually written in component parts or units constructed in isolation for integration at a later stage 
* Each of those units of code will relate to certain function or area and be tested by developer to make sure it work. 

--

#Integration Testing 
* Purpose is to expose defects in the interfaces and interactions between integrated component or system 
* The test objects are essentially the interface doe 

**The types of integration testing are:** 

##Big Bang Integration
* All units are linked at once resulting in a complete system 
* Difficult to isolate errors since no attention to verifying interfaces across individual units 
* Introduces risk that problems may only be found late in the project 

##Top Down Integration 
![Top Down] (http://www.softwaretestinggenius.com/photos/ISBF13A.JPG)

System is built in stages, starting with components that call other components.
  
Testers evaluate components interfaces, starting at the **top**. We test interactions with a substitute component called a stub. We use stubs because the component we want to test may not be integrated yet.

**Stub** - **Passive** component, called by other components. 

In the diagram above the stubs would be 4, 5, 6, & 7

###Advantages   
* Useful creating software intended to be generic  
* this will allow for early demonstrations of the products functionality   
* may help identify requirements changes and issues   

###Disadvantages   
* stubs can create a lot of work  
* stub definition can be difficult   
* reproducing test conditions may not be possible  
*  

##Bottom Up Integration
![Bottom Up] (http://www.softwaretestinggenius.com/photos/ISBF13B.JPG)

Components are integrated from the bottom up 

Components that are not in place that actively call other components are substituted using **drivers**

**Drivers** - **Active** component, controlling other components

In the diagram above the drivers would be 2 & 3

--

#System Testing 
* Tests functionality from an end to end perspective 
* Focuses on the whole system in a representative live environment 
* Usually carried out by a team independent of the development process
* Test functional and non functional requirements

--

#Acceptance Testing 
* Testing to provide end users confidence that the system function according to user expectations
* Often done by customers or users of the system 
* Key purpose is to demonstrate system conformance to customer requirement and operational processes

**Contract and regulation acceptance testing**

Contractural - Acceptance criteria outline in a contact   
Regulations - Certain industries have rigid regulation that must be abided by:  

 - Governmental   
 - Legal  
 - Safety Reasons  
  
Ignorance is not a defence the can be used. It is your responsibility to work within the boundaries of the law
 
**Alpha and beta acceptance testing**   

Alpha - Testing performed on site    
Beta - Testing done off site by potential users of the system   

**User acceptance testing**  

* Tested by user representative 
* Checks the system meets business needs
* A form of validation 
* normally happens at the end stage or development system 

**Operational acceptance testing**

* Checks the processes and procedures are in place to allow the system to be used and maintained. Includes checking 
	* Back up facilities 
	* Procedures for disaster recovery 
	* Training for end users 
	* Maintenance procedures 
	* Data load and migration tasks 
	* Security procedures 

--
	
#Test types
**Functional Testing**    
**Non Functional Testing**  
**Structural Testing** 
**Testing after code has been changed**

-- 

##Functional Testing 
* Can the system do what I need it to do 
* Testing of the functions of system. 
* Verifying a specific action or function of the code works 

Also called specification based testing i.e testing against a specification 

##Non Functional Testing  
Testing behavioural aspects of the system 

* Installability 
* Maintainability 
* Performance 
* Load handling 
* Stress handling 
* Portability 
* Recoverability 
* Reliability 
* Usability 

**Black Box Testing**  
Testing, either functional or non-functional, without reference to the internal structure of the component or system 

##Structural Testing 
Testing the code itself 

* How to code makes the functionality work. What is happening  "under the hood"
* Can be carried out at any test level 
* decision coverage 
* state coverage 

**White Box Testing**  
Testing based on an analysis of the internal structure of the component or system.

#Testing related to changes

**Retesting (Confirmation)**

* After a defect has bee fixed the software should be retested to make sure the defect does not occur again 

**Regression Testing** 

* carried out on every other part of the system to check that a fixed defect hasn't changed other parts of the system 
* repeated resting of already tested program 
* performed when software or environment is changed
* based on risk 
* performed at all levels (functional, not functional, structural) 

*Testing certain parts of the system make sure there are no unintended consequences of a defect fix*

###RCRCRC 
**Recent**   
**core** - essential functions must continue to work  
**risk** - if a new feature is added analyse which part of the system may be at risk  
**configuration** -   
**repaired** - how new bug fixes can likely effect the system   
**chronic**  - how some area may be sensitive to break, when a new feature or bug fix is introduced   

--

#Maintenance Testing 
Testing in a live environment when there has been: 

* Modification 
* Migration
* Retirement of software 

Also
  
* They help estimate the amount of re testing and regression testing  
* What are the possible consequence 
* What areas will remain unchanged 

#Test Harness 

Test harness or automated test framework is a collection of software and test data configured to test a program unit by running it under varying conditions and monitoring its behavior and outputs. It has two main parts: the test execution engine and the test script repository.