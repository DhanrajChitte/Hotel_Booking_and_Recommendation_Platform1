# Hotel_Booking_and_Recommendation_Platform1
  This Repository Contents the Frontend,Backend,Database file and the MarkDown(MD) files for the API for the system                  Hotel_Booking_and_Recommendation_Platform.

# Share the ScreenRecoder Link to See the Demo of the System:
  You can see the how system work from here:
  https://drive.google.com/file/d/1EXDD4YHfL0h4a9oHockroyQUz52_gERE/view?usp=sharing

# Technologies Used:
1) Frontend:-HTML,CSS,JavaScript(JS)  (Basic UI)
2) Backend:- NodeJS,ExpressJS (Main Focus)
3) Database:- MySQL (Main Focus)

 The Repository Content the 4 sub folders such as the Frontend,Backend,MarkDown(MD)Files,Database.

# Database:
  1. Database folder content file Hotel_Booking_and_Recommendation1.sql in which the I have export the system database including        all the tables Users,Hotels,Visits,Booking.
  2. For Exporting Data into SQL File Command: mysqldump -u root -p Hotel_Booking > Hotel_Booking_and_Recommendation1.sql.
  3. For Importing SQL File into the Database you can use this command after the create the database name Hotel_Booking:-
     mysql -u root -p Hotel_Booking < Hotel_Booking_and_Recommendation1.sql.

# Backend 
   (I have also upload the package.json file from which modules have used of the NodeJS and for the running the server of   the       node use the Main.js file because all the APIs inegrated on this file for the runnung server one time only).
# In the backend part of the system there are total 6 APIs such as
   1) Registration API for Customer: This API successfully register the customer in the system if the customer fill all the           necessary fields correctly otherwise give the error message because Validation for the Email,Password,Phone Number and Customer    Name.API in file RegistrationCus.js.
   2) Login API: This API for the customers whose already register in the system.By taking emailid and password from customer if      match then login otherwise not.API in the file Login1.js.
   3) Search Hotels API: This API give the customer opportunity to search the hotels that they want.Customer Search the Hotel by      using Hotel name,area,city,state,rating and the price and see the result if result match.API in the file Search.js.
   4) VisitsRecords API: This API give the hotel details of the hotel and go to the home page of the hotel and track the visits       status of the Customer and save.API in the file VisitRecords.js.
   5) Hotel Booking API: This API responsible for the Book the hotel.If customer give the payment partial/complete then Booking       Completed.Otherwise only fill the necssary details then Booking Draft.API in the file Booking.js.
   6) Hotels Recommendation API: This API give the customer Recommendation of the hotels other than the that they already visited     home page of the hotel or already draft/completed booking before.API in the file Recommendation.js.

# Frontend :
  In the Frontend Part there are total 6 Screens:
  1) Registration Page: Page take the input data from the user and register if successfully register go to the Search Hotels Page    Directly.The CSS and JavsScript files for this page are seprate Style.css and Script.js respectively.
  2) Login Page: If the user have alredy account then login from this page otherwise go to the SignUP page from this page.If login   succeful go to the search hotels page.
  3) Search Hotels Page: In this page the customer search the hotels that they want according same criteria from the API.In this     page after the searching the hotels customer see the hotel listes and then after click on particular hotel customer go to the      hotel home page. in this page Hotels Recommendation option available on clicking this go to the recommendation page.
  4) Hotel Details Page: In this hotel home page customer see the datail of the hotel and from here go to the Booking page           otherwise the back to the search hotel page.
  5) Hotel Booking Page: In this Page the form will display after filling the form user can payment or not if user done payment      then the booking completed otherwise status of the booking is draft.If the booking draft from this page user come back to the      search page.
  6) Recommendation Page: The Recommendation Hotels option show in the Search Hotels page and click on this the recommended hotels   will seen and proceed further.

# MarkDown(md)Files :-
  In the md files there are 6 md files for the 6 APIs mention above and all the functionality and features for the APIs mention      briefly on those Files.
   1) RegistrationCus.md
   2) Login1.md
   3) Search.md
   4) VisitsRecords.md
   5) Booking.md
   6) Recommendation.md
  

 
