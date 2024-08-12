## Login API for  Customer in Hotel_Booking_and_Recommendation_System
   POST/api/Login1

## Request Headers
   Content-Type:application/json

#### Request body
   {
    Email:"String",
    Pass:"String"
   }

## Response
  200-Success(OK)

Body (json) 
{ 
    Message:"Login Successful"
    user_id(userToken):Integer, 
    email:"String",
    username:"String"
    Password:"String",
    Time: "YYYY-MM-DD HH:mm:ss in Asia/Kolkata timezone"
}

404 - Not Found

400 - Bad Request 
      {
      Error:"Invalid Password or Email ID"
      }

500 - Internal Server Error
     {
      Error:"MySQL query error"
     }