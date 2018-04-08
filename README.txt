Halal-Bot Is Smarter Than You!

Authors: Matthew Kearns and Ahmed Youssef.


Brief Explanation:

This is a simple expert system that learns information to answer questions
about its behavior. It uses forward-chaining to learn new rules given 
user-supplied rules and variables (either root or learned), and it uses 
backward-chaining to create explanations for its behavior given the values 
of the variables in the system and the learned rules.

The difference between a root variable and a learned variable:

A root variable is a variable whose truth value is known by the
user, and the user can set its value to either true or false. The
truth value of a learned variable, however, depends on the rules of
the system and the values of the root variables that it depends on.


Usage Instructions:

	1. Teach [-R/-L] Var = String
	
		Teaches the system the type and value of a variable.
		
	2. Teach Var = [True/False]
	
		Teaches the system the truth value of the variable.
		
	3. Teach Expression -> Var
	
		Teaches the system a new rule.
		
	4. List
	
		Lists the values of all root and learned variables, and
		lists all of the current rules and learned rules in the
		system.
		
	5. Learn
	
		Creates new rules based on rules already supplied in the system
		and updates the truth values of the variables based on the rules.
		
	6. Query Expression
	
		Query returns the truth value of the expression based on all of 
		the current rules and variables in the system.
		
	7. Why Expression
	
		Why gives an explanation of why the user-supplied expression is true
		or false given the current rules and variable values held by the
		system.
		
	Key:
	
	-R = root variable
	-L = learned variable
	Var = user-defined variable name
	String = A string of the form "Today is Monday" or "Matt likes ice cream"
	Expression = Any valid expression of the form A&B->C or (!((A|B))&C)->D

