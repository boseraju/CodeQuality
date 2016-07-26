# CodeQuality

Good Code Quality



 Meaningful Names:
	While writing variables, functions, Classes and packages follow simple rules for creating meaningful Names.
	
 Rules:	
	
Rule1:

Use Intention-Revealing Names:
	
		Names should reveal intent of Usage. 
		
		for eg:   int i = 46         // age of a person
				  String value = "user123"  // username
				  
	    in the above example variables i,value reveals nothing. 
        we should choose these variable names as below to make them more meaningful.
		
		 int ageOfPerson = 46         
		 String accountUserName = "user123"  
		 
		 
		 the below code snippet pulls all the accountNumbers(checking,savings,kids etc..) associated to a given Customer by his/her username. 
		 
		 public Set<String> getAccounts(String customer){		 
		    Set<String> hset = new HashSet<String>();
			hset = getAccountsFromDb(customer);
			
			.....
		    return hset;
		 
		 }
		 
		 But by looking at the code it is difficult to understand what's going on.
		 we can change the above code to meaningful like below.
		 
		 
		 
		 public Set<String> getAccountNumbersAssociatedToCustomer(String userName){		 
		    Set<String> bunchOfAccountNumbers = new HashSet<String>();
			bunchOfAccountNumbers = getAccountNumbersFromProfile(userName);
		    
			....
			return bunchOfAccountNumbers;
		 
		 }
		 
		 
		 Rule2:

Use Pronounceable Name:

	Class Cust {
	  
	  private String fm;
	  private String lm;
	  private float bal;
	  private boolean lbind;

	
	} 
	
	
	to 
	
	Class CustomerAccountInfo {
	  
	  private String firstName;
	  private String lastName;
	  private float  currentBalance;
	  private boolean lowBalanceIndicator;

	
	} 
		 
		 
		 
		 
		 
		 
		 
		 
		 
		 
		 
		 
		 
