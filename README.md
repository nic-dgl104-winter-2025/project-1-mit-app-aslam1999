[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/so8F8uYz)
# MIT App Inventor Project

**Project Documentation of Donation App**

1. **Introduction**
   
   The Donation App is a mobile application designed to allow users to make donations of food, clothes, groceries and money. It provides a simple and user-friendly interface for donors to submit their contributions and view past donations. The app is built using MIT App Inventor, a visual programming platform for creating Android apps.

2. **Objectives**
   
   -To create a platform that makes it simple for people to contribute goods or cash.
   -Donation records will be kept and shown for future use.
   -To offer a smooth, user-friendly navigating experience.

3. **Features**
   
   1. **Login Page Screen**: Allows users to login using there credentials(I have used username: Aslam, Password: 12345 to test).
   2. **Home Screen**: Allows users to select the type of donation they want to make.
   3. **Donation Form Screen**: User can input the donation details.
   4. **Donation List Screen**: Displays the record of past donations.
   5. **TinyDB Storage Component**: Stores the donation records locally on device.
   6. **Dynamic UI**: Hides/Shows relevant details as per donation category.

4. **App Structure**

   1. **Screen 1: Login Screen**
        - TextBox for username and password.
        - Button to submit the credentials and login.
        
   2. **Screen 2: Home Page** 
        - Buttons for donation categories: Food, Clothes, Groceries, Money.
        - Button to view past donations.
    
   3. **Screen 3: Donation Form**
        - TextBoxes for name, item, quantity, and amount.
        - Spinner for selecting donation category.
        - Button to submit and save donation details.
    
   4. **Screen 4: Donation List**
        - ListView to display all donations.
        - Button to return to the home screen.
  
  (Note: Home screen is created first and later remembered of login page and created it later. As a result, The first screen technically on app is home screen bymistake. You can redirect and start from login page.)

5. **Components Used**
   1. **UI Components**
        - **Labels**: For displaying text (e.g., "Welcome to Donation App").
        - **Buttons**: For navigation and actions (e.g., "Login", "Submit Donation").
        - **TextBoxes**: For user input (e.g., name, item, quantity, amount).
        - **Spinner**: For selecting donation categories.
        - **ListView**: For displaying donation records.
     
   2. **Non-Visible Components**
        - **TinyDB**: For storing and retrieving donation records.
        - **Notifier**: For showing confirmation message. 

6. **Block Logic**
   1. **Screen 1: Login Screen**
     - `Btn_Login.Click` Opens screen 2 if username and password are matched. Else set `Label_Message.Text` to "Invalid Username or Password" message.
  
   2. **Screen 2: Home Page** 