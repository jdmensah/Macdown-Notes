#BDD:Specification by Example 

##SBE
Specification by Example (SBE) is a technique that enables product owners, business analysts testers and programmers to eliminate common misunderstanding about business requirements. 

###Advantages
* Implementing changes more effectively 
* higher product quality 
* less rework 
* better work alignment

###SBE Process Pattern
* Deriving scope from goals 
* specifying collaboratively 
* illustrating using examples 
* refining the specification 
* automating validation without changing specs 
* validating frequently 
* evolving a documentation system 

![](http://hsto.org/storage2/00f/0a0/534/00f0a0534e75bcb954a8e05e62acf0ee.png)

Business goal are similar to epics, define scope from goals (user stories), you end up with key examples (refined user stories) 

A **living document** or **dynamic document** is a document that is **continually edited** and updated.

##Deriving Scope from Goals 
* Not reliant on product owners to define scope 
	*  using the teams initiative 
* being with a business goal 
	* the client will tell you what the goals are
* work as a team to derive the scope 
	* using the teams initiative
	* working as a team 
* keeps the business goal at the forefront 
	*  ensure every one is working to achieve the business goal 
* leads to a description of the scope 
	* there may be a cheaper or different way to define the goal

##Specifying Collaboratively 
* Happens just-in-time 
* developers, testers and product owners 
* specify requirements together 
* works with traditional requirements 
* works with user stories and acceptance criteria 
* creates shared ownership 

##Refining the Specification 
* Remove extraneous details 
	* removing details that are not necessary 
* add more detail 
	* adding relevant details where it is missing 
* improve the language
	* readability of the user story 
* creates acceptance criteria 

##Automating Validation 
* Automate acceptance tests based on these 
* acts as a basic regression and UAT framework
* provides quick feedback on whether the right product is being built 
* becomes an executable specification 
* we can then validate that the production meets the specification frequently 

The feature is the user story 
Each scenario is a acceptance criteria 

##Evolving Living Documentation 
* Frequently validated = Up-to-date
* As reliable as the code, but easier to read 
* support staff can find out what the system does 
* developers can target new development 
* testers can derive tests 
* business can analyze the impact of change 
* free regression testing 
* we can keep it all in VCS

--

#ATDD & BDD - Acceptance Test Driven Development & Behaviour Driven Development 

###ATDD
More traditional term using UAT to drive the development. the tests drive

###BDD
associated with cucumber. using the expected behaviour and business value to drive development.

describes solely the behaviour 

###SBE 
the part of BDD that involves using examples to specify requirements 

###Convergent thinking vs Divergent thinking 
![](https://cucumber.io/images/blog/divergent-convergent-thinking.png)

###Convergent 
Convergent thinking is a problem solving technique involving the bringing together different ideas from different participants or fields to determine a single best solution to a lucidly defined problem. In other words, this is a kind of thinking that concentrates on finding out the single best or frequently, correct solution to a problem or answer to a question. 
