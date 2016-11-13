#Exploratory Testing 

##Test Strategy

* Does the software behave as expected under the conditions its supposed to be able to handle 
* Are there any risks 

##Essential Element 

* Designing 
* Executing 
* Learning 
* Steering 
* Time boxing 

where   
what equipment we need   
what information are we seeking   - Charters 

target  
resource   
information   

##Charters 

* often generated during conversations
	* Agile Ceremonies 
	* Requirements gathering meetings 
	Conversation with BAs, stakeholders and developers   
* often generated when executing test cases 
* must include
	* the target area 
	* the resources/techniques/tools we'll use  
	* the information we seek 
* should not be too specific 
* should not be too broad 

##Talk to stakeholders

Where can we get ideas 

* Stakeholders questions and comments
	* What will happen if we add 300 more products in the future?"
	* could a user ever see another users private profile
* the source code 
	* // TODO: don't know why this works, but it does. don't touch it need to fix at some point
* developer comments 
	* "The profile image upload is a bit flaky because the redis write queue is being weird. it works most of the time though"
* your own findings and knowledge of the system 
	* "that video behaved strangely when i put the iPad in landscape model. i wonder if that problem exists anywhere else?"
* existing defect and defect reports 
	* Particularly areas where defects are clustered

#Observation 

* Be alert to subtle cues
* try unusual things 
* use monitoring software to look for the unusual 
	* High cpu/memory usage
	* unusual network traffic
	* strange HTTP requests/responses 
	* strange filesystem read/writes
* look at Console & server logs


Session Sheets