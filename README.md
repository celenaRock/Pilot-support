# Pilot-support

Pilot Support and the Process of QA
1.	Was the customer justified with their complaints?

A: Absolutely. Apparently, nobody told the customer this wasn’t the final product.

2.	Did the QA do a good job responding to the customer’s complaints?

A: The QA did an okay job responding to the customer’s complaints. Too much justification and not enough listening and attempting to try to figure out how they ended up here in the first place. It’s good to address customer dissatisfaction, but better to avoid it in the first place.

3.	Would you address them in a different way?

A: I would definitely address the customer in a different way. If the customer is just now hearing that what they’re seeing is a prototype, it makes the customer think we’re a bunch of amateurs. The progression of product releases should have been communicated clearly to all stakeholders well in advance. The testing could have been preceded by a showcase session to set expectations. Better still would have been to limit releases to more fully functional versions.

4.	What information would you need to adequately respond to their concerns?

The original specifications and any further changes arising from other communications with the customer.
Customer’s Feature Checklist:
1.	Enter all required data, including email
2.	Save entered data
3.	Search for data
4.	Log in and log out
5.	Attractive styling
Testing Document Outline:
1.	What are we testing?
We are testing the data entry, save, and cancel functions
2.	How long will we test?
Until all tests are complete or allotted time ends
3.	Are there pieces we won’t test?
Connectivity to database will not be tested
4.	How do we plan to test?
We will test by changing each of the employee fields and entering, then doing the same and cancelling.
5.	How will we know we’re done testing?

We will know we are done when all functions have been tested.
Testing:
	Basic functionality is good. Data is not saved after refreshing browser.
Test Document:
Purpose: To test the XYZ Company Employee Manager app for functionality
Application Overview: The Employee Manager app allows the user to enter employee data in the form of an employee card containing field for name, phone number, and employee title. Employees are given an employee ID number that cannot be changed.
Testing Scope:
	In-Scope:
	
Entering data, saving data, basic functionality, security check
Test 1: Enter null data 
Result: Entering blank name deletes employee but leaves blank where employee name was. Entering blank data in other forms has no effect. 

Test 2: Entering incorrect phone number
Result: Entering overly long string of numbers or entering letters is not prevented, although console appears to detect “Uncaught RangeError: Maximum call stack size exceeded”
Test 3: Entering long string length in title
Result: No limits on string length in title

Test 4: Entering special characters
Result: Special characters can be entered for name, phone number and title without restriction

Test 5: Using cancel button
Result: Cancel button works

Test 6: Certificate is valid and trusted, connection is secure, resources are served securely

Test 7: Chrome Lighthouse test returns 100%. Suggests removing non-functional JavaScript for 0.15s saving

Test 8: General visual
Result: Employee ID 4 is actually -4
	-Out of Scope:
		-System Integration testing
		-Regression testing
	-Items not tested: None	
	
Metrics: 5 out of 5 
Test Environment and Tools: Windows 11, Chrome 96.0.4664.45

Lessons Learned:
	-Chrome has some testing tools built in
	-Testing may uncover unexpected side effects that force you to go back and redo the tests
	
Recommendations:
	-Add email field
	-Change Employee ID 4
	-Restrict entry length and use of special characters
	
Best Practices:
	-Restricting entry of special characters prevents use of unwanted scripting commands and reduces the likelihood of bad data being entered into the system either intentionally or unintentionally.
	
Exit Criteria: 
	-When all functions have been tested or allotted time is complete
Conclusion:
	-Employee Manager is a solid performer that needs a few changes to achieve perfection. Add an email field, make all the entry fields sensitive to string length and content, disallow entering null data.
	
Definitions, Acronyms, Abbreviations: N/A


