# Chapter 10 Forms: Reactive form - login

## Objectives

- Add a login form
- Update Display when user is logged in

## Steps

1. Continue working in your **my-angular-albums** project. If you haven't completed previous exercises, you can copy the src directory from the solution in the last exercise over yours.

1. In your project navigate to your app/shared folder and app/login folders and delete them.

   ![](../screenshots/2-delete-shared-folder.png)

 
2. Make sure the angular100-labs project is open in VS Code and navigate to the same folder as this README.md. Copy the shared and login folders from here into your project **app** directory.

   ![](../screenshots/2-copy-shared-folder.png)


3. In **app.module.ts** in the @NgModule decorator of core, import **ReactiveFormsModule** to be able to create a reactive form in the LoginComponent. Make sure the import of the module as an ES6 import is at the top of the file.

   ![](../screenshots/2-import-reactive.png)

4. Copy the contents of the login directory in this README file folder over the contents in your login directory.
   
5. View the new versions of files in the **/login** folder in the VS Code editor. 
    1. In the **login.component.html** notice the use of formGroup and how the error messages, and submit are worked with conditionally.
    2. In the **login.component.ts** file, notice the work with FormBuilder, and setting up of email and password along with Validators. Validators.required is built in, and ValidationService.emailValidator and ValidationService.passwordValidator are custom. 

6.  With these changes in place your code should now work. Clicking on login should bring up the login page. Supplying the username of user and the password of root should log you in. 

## Bonus
1.  Use Reactive form to add a new album. 
    1.  create a button Add Album to the listing
    2.  use ReactiveForm to take in input
        1.  You can copy from previous exercise template but need to change to be reactive
    3.  create and call a new album service method that uses http.post
   