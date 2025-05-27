In this project you complete the script for a web form that collects billing and shipping information. Because the shipping address and billing address are often the same, this form will include a checkbox to copy the shipping address values into the corresponding billing address fields. Also, instead of using browser error bubbles to report invalid data, display the text of the error message in a box at the bottom of the form and prevent the browser from showing error bubbles in response to validation errors. A preview of the form is shown in figure 6-40. 
1. Use your code editor to open the project06-03_txt.html and project06-03_txt.js files from the js06project03 folder. Enter your name and the date in the comment section of each file and save them as project06-03.html and project06-03.js. 
2. Go to the project06-03.html file in your code editor and link the page to the project06-03.js file, deferring loading of the script. Study the contents of the file and note field names associated with each input element within the form. Save your changes to the file. 
3. Go to the project06-03.js file in your code editor. Below the comment section declare the useShip variable in reference to the element with the id “useShip”. Add an event listener to useShip to run the copyShippingToBilling() function when clicked. 
4. Create the copyShippingToBilling() function that copies values from the shipping fields to corresponding billing fields. Within the function, insert an if statement that tests whether useShip is checked and if it is, do the following 
      - Set the value of the firstnameBill field to the value of the firstnameShip  field.
      - Repeat the previous step to set the value of the last nameBill, addressBill, address2Bill, cityBill, countryBill, codeBill fields to the values of their corresponding fields in the shipping part of the form 
      - Set the selectedIndex property of the stateBill field to the value of the selectedIndex property of the stateShip field. 
5. Below the copyShippingToBilling() function do the following:
      - Declare the formElements variable and using the querySelectorAll() method store within it a node list corresponding to elements selected with “input (type=’text’)”. 
      - Declare the fieldCount variable with a value equal to the length of the formElements node list.
      - Declare the errorBox referencing the element with the id “errorBox”.
6. Create a for loop that iterates through each element in the formElements node list and for each element apply an event listener that calls the showValidationError() function in response to the invalid event. 
7. Create the showValidationError (evt) function and add the following commands to it:
      - For the event object, evt, apply the preventDefault() method to prevent the browser from applying the native browser tools to respond to invalid data.
      - Set the textContent property of the errorBox to the text string “complete all highlighted fields”.
8. Save your changes to the file and then open js06-03.html in your browser. 
9. Verify that you can copy shipping address information to the billing fields by clicking the same as shipping address box. 
10. Verify that you cannot submit the form until all data fields are completed and that the validation errors appear in the error box below the form. 

