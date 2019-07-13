# Import-Marvel
Powershell script and .CSV file that allows you to import marvel characters as users into Active Directory

Script will:
1. Add users into Active Directory
2. Add users to appropriate groups based off of `marvel_users.csv`.
3. Set Service Prinipal Names (SPN)'s for users `thor` and `ironman`. 


To run:
1. Download 'marvel_users.ps1' and 'marvel_users.csv'.

2. Change domain name to match personal enviroment's domain.
 
**Note:** This will need to be done in both files. 	

-  Inside of 'marvel_users.ps1' on line: 60, 79, & 80
	
-  Inside of 'marvel_users.csv' for each user in the 'ou' section

**Example:** "CN=thor,DC=example,DC=com" if desired domain is 'example.com'
		
3. Change the path to which 'marvel_users.csv' is located on line: 6 for 'marvel_users.ps1'

4. Run ./marvel_users.ps1 

