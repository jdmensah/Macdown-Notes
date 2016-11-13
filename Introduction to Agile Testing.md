#Introduction to Agile Testing 

###What is an Agile Tester 

* liaise with developers 
* tests components of the system 
* write specifications for tests 
* collaborates with technical and business people 
* uses tests to document requirements (BDD, living documentation) and drive development 
* embraces change 
* exploratory Testing
	* scope - what are you going to test 
	* time-boxed - how long will you spend testing 
	* tools needed - how will you perform the test 
	* goal - what are you going to look for 
* executing manual test cases 
* pairing with developers to write automated functional acceptance and unit test 
* recognizing possible problems when planning 
* writing acceptance tests with BA and PO before coding starts
* writing and executing 'ility' tests 

##Deliver Business Value 

###The Right Mindset 
* See the big picture 
* view the app from a user and customer perspective 
* help the product owner express their requirements properly 
* don't just test - innovate, learn and solve whatever problems need solving 

##Test Strategy
> A high-level description of the test levels to be performed and the testing within those levels for an organization or programme (one or more projects).

* Risk mitigation - taking steps to reduce adverse effects 

Defect Tracking - identifying and monitoring defects 

##Technical Debt 
* Carrying over tasks into the next sprint 
* Bugs to fix 
* performance improvements to make 
* security fixes 
* usability problems to solve 
* making the code more maintainable 
* refactoring 
* predicted edge-cases and 'open loops'



##Agile Testing Quadrants

![Agile Testing Quadrants](http://lisacrispin.com/wp-content/uploads/2011/11/Agile-Testing-Quadrants.png)

##Q1: TDD 
Write the tests, then build to system to pass the test 

Write a failing test  
test is green 
refactor 

###Benefits 
* Improves quality by focusing on requirements before coding 
* keeps code clearer, simple and testable 
* provides documentation for other /new team members 
* provides reparable tests fro regression 
* enables repaid change 

#Unit Test 

#What Might a Tester/ SDET do ?

###Project/ Release Planning 
* Understand the product 
* develop a test strategy covering q1-q4
* consider possible blockers 
* work with DevOps and Developers to build a pipeline and infrastructure 

###Sprint Planning 
* Work with BA/PO to refine acceptance criteria 
* identify q3 and q4 testing that might be required in the sprint 
* work with the BA/PO to define scenario-based acceptance criteria for automation 

###During the Sprint
* pair with developers on unit test 
* exploratory testing 
* write manual test cases and prepare test data 
* manual q2,q3 and q4 tests 
* execute and report on manually triggered automated integration tests 
* develop automated q2/3 tests 
* develop automated q3 and q4 tests and required 
* maintain the test framework 

###Prior to Release 
* Manual regression test if required 
* manual tests on the critical path 
* execute and report on automated tests on the release staging environment (production like) 

