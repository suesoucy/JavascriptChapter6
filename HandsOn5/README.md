You have been given a web form that is to be used to register attendees at a conference. However, there are errors in the JavaScript program that calculates and reports the total costs of the registration. You have been asked to locate and fix the errors in the code. A preview is show in figure 6-42. 
1. Use  your code editor to open the project06-05_txt.html and project06-05_txt.js files from the js06proejct05 folder. Enter your name and the date in the comment section of each file and save them as project06-05.html and project06-05.js .
2. Go to the project06-05.html file in your code editor and in the head section add a script element to load the project06-05.js file, deferring it until the entire page is loaded. Study the contents of the file to become familiar with the structure of the HTML code. Save your changes to the file. 
3. Return to the project06-05.js file in your code editor. Comments have been added to help you interpret the code in the file. 
4. The first part of the code uses an anonymous function to load several event handlers to calculate and recalculate the shopping cart as different form fields lose the focus. There are several errors in this anonymous function.
5. The sessionTest() function is used to confirm that the user has selected a session to attend at the conference. If the user did not select a session, the form should be invalid. Locate and fix two errors in setting up the custom validation message. 
6. The calcCart() function is used to generate the contents of the shopping cart and calculate the total cost of registration. Within this function there are errors in determining the index of the chosen session, whether the user checked the media checkbox, and in the display of the total cost of the registration. Locate and fix all three errors. 
7. Save your changes to the file and then open project06-05.html in your web browser. Verify the following:
      - When you enter text into the form fields and tab out of the input boxes, the shopping cart text automatically updates to show your data entry. 
      - As you select different conference options, the total cost of the conference automatically updates. 
      - The total cost of the conference is displayed in U.S. currency.
      - If you attempt to submit the form without entering all required data, the form will be rejected. 

