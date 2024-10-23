
## Lab-1 : Unprotected admin functionality

### Goal: Find the Unprotected admin panel and delete the user carlos

### Analysis: 

- Start by visiting the homepage of the shop, where you can see various products listed.
- Next, add /robots.txt to the URL: https://0a6c00050384ce4584bf8a2100b100c0.web-security-academy.net/robots.txt
- The robots.txt file reveals a disallowed path: Disallow: /administrator-panel
- Navigate to the following https://0a6c00050384ce4584bf8a2100b100c0.web-security-academy.net/administrator-panel
- This brings you to the admin panel, where you can view all user accounts. To solve the lab, simply delete the user "carlos" by selecting the delete option next to his name.

By doing this, you successfully complete the lab challenge!!!

## Lab-2 : Unprotected admin functionality with unpredictable URL

### Goal: Find the Unprotected admin panel that is located at an unpredictable location and delete the user carlos

### Analysis: 

- Start by visiting the homepage of the shop, where you can see various products listed.
- We can find the link to the admin panel in the source code of the homepage of the lab, which is adminPanelTag.setAttribute('href', '/admin-6xaa5o');
- That will be the location ofthe admin panel, where we can access the users and delete them.
- Navigate to the following https://0a6c00050384ce4584bf8a2100b100c0.web-security-academy.net/admin-dif9jv
- This brings you to the admin panel, where you can view all user accounts. To solve the lab, simply delete the user "carlos" by selecting the delete option next to his name. 

By doing this, you successfully complete the lab-2!!!

## Lab-3 : User role controlled by request parameter

### Goal: Solve the lab by accessing the admin panel and using it to delete the user carlos.
User can log in to their own account using the following credentials: wiener:peter

### Analysis: 

- Log in as a regular user using valid credentials.
- Inspect the user's cookies and find the "admin" cookie with a value of false.
- Change the value of the "admin" cookie to true and refresh the page.
- After refreshing, notice that the user now has admin privileges and can access the admin panel.
- Click on the admin panel link to navigate to the user accounts page.
- To complete the lab, delete the user account named "carlos" by selecting the delete option next to his name.

By doing this, you successfully complete the lab-3!!!





