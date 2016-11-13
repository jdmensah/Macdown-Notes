#Continuous Delivery
[Useful Link](https://blog.assembla.com/AssemblaBlog/tabid/12618/bid/92411/Continuous-Delivery-vs-Continuous-Deployment-vs-Continuous-Integration-Wait-huh.aspx)

#Pipeline 
push to git, runs automated tests, runs unit tests, 

##Continuous Integration 

* integrate with the working system so far
* run automates tests on every push 
	* used to ensure quality  
* have a visible indicator of when the build is broken 

**Every time a new part or feature of the product is completed we add it to the current built**

Keep on integrating new stuff to build 

##Pre-requisites for CI

* Version Control 
* An Automated Build 
* Automated Tests 
* Agreement from the whole team 

##CI Tools

* Drone.io
* Teamcity 
* Travis 
* Jenkins 

##Continuous Delivery

* use CI to integrate into a production like system 
	* mimics that production environment 
	* accessible by other people
	* used for testing 
* test act as 'quality gates'
* you don't push to production just yet, it will go to production like first 
* **ends at the production like gate **

![](https://blog.assembla.com/hs-fs/hub/365/file-1239046021-png/images/cd_process_diagram-resized-600.png?t=1477939274289&width=622&height=332&name=cd_process_diagram-resized-600.png)

##Continuous Deployment 

* deploys all the way to production - doesn't go to prod like 
* Build pipelines are often complex 
* **ends at the production gate **

##Code Coverage Metrics 

* Bug counts 
* amount of unit test created 
* how much code in the system is covered by unit tests 
