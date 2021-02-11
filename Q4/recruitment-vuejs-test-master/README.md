## Debug
-. When i want to run, i need to install npm.
-. When I run it for the first time, there is an error:
    1. mapState is defined but never used
    2. INCREMENT is define but never used
    3. error is defined but never useed.
    
-. I open it for the second time after I closed it before, it can run. then i checked where the error was in the file.
-. Error is in the User.vue
-. There are import mapState and INCREMENT from the directory, but they are not used in the function.
-. After the file runs successfully, the screen appears "User list, number 0, and Users"
-. I see something wrong in the appearance, then I checked on User.vue
-. The display should have output: 
    1. Name
    2. Email
    3. Phone
    4. Website 
    based on data that has been stored in the "state" but i can't fix it because i'm still learning about Vuex. I've never used that

    Thank you very much