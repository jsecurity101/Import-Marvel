# Import-Marvel
Powershell script and .CSV file that allows you to import marvel characters into Active Directory


To run:
1. Download 'marvel_users.ps1' and 'marvel_users.csv'.

2. Change domain name to match personal enviroment's domain.
 
**Note:** This will need to be done in both files. 	

-  Inside of 'marvel_users.ps1' on line: 36
	
-  Inside of 'marvel_users.csv' for each user in the 'ou' section

**Example:** "CN=thor,DC=example,DC=com" if desired domain is 'example.com'
		
3. Change the path to which 'marvel_users.csv' is located on line: 6 for 'marvel_users.ps1'

4. Run ./marvel_users.ps1 

5. After script is ran for the first time, will be able to call it by inputting: Import-Marvel
