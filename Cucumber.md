#Cucumber 

Feature: Something   
	Free text 
			
Background:  (what ever follows next is shared by all the following scenarios)
	Given I am logged in 
	
Scenario: Something  
	Given ....  
	And  ....  
	When ....  
	Then ....  

> Each scenario **must** make sense and be able to be executed *independently* of other scenarios

##Gherkin Keywords 

* feature 
* background 
* scenario
* give
* when 
* then 
* and 
* but 
* * 
* scenario outline 
* examples

Writing Good Feature files 
Imperative and declarative 

##Shared Understanding 
* shared ownership pf code 
* good code comments 
* coding standard 
* collaboration 
* code for others to read 
* system metaphor 

##Bad Cucumbers 
* Flaky/flickering scenarios
	* unreliable scenarios - those that pass sometimes
* Brittle scenarios
* Slow scenarios 
* Bored stakeholders 
* Leaky scenarios 

#Bad and Good Cucumber Example 
```
Bad Example
Scenario: Create an invoice
    Given I am a signed in user with role: admin
    And a client "Test Client" exists with name: "Test Client"
    And a project "Test Project" exists with:
        | name   | "Test Project"       |
        | client | client "Test Client" |
    And an issue "Test Issue" exists with:
        | project | project "Test Project" |
        | name    | "Test Issue"           |
    And a work_unit "Test Work Unit" exists with:
        | issue        | issue "Test Issues" |
        | completed_on | "2011-08-24"        |
        | hours        | "7.5"               |
    And I am on the admin invoices page
    Then I should see "Test Client"
    And I follow "Test Client"
    And I fill in "invoice_id" with "abc"
    And I press "Submit"
    Then I am on the admin invoices page
    And I should not see "Test Client"


Good Example
Can be refactored to:
Scenario outline: Submit an invoice
    Given I am signed in with admin privileges on the admin invoices page
    And <test client> exists with related <test project>, <test issue>, <completed_on> and <hours>
    Then I should follow <test client>
    And I can submit after filling in <invoice_id>
    And <test client> is no longer on the admin invoices page
    Examples:
        | test client | test project | test issue | completed on | hours | invoice_id |
        | Test Client | Test Project | Test Issue | 2011-08-24   | 7.5   | abc        |

```

