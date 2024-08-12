## Registration/SignUp API for  Customer in Hotel_Booking_and_Recommendation_System
   POST/api/Sign_Up 

## Request Headers
   Content-Type:application/json

#### Request body
   {
    Email:"String",
    CustomerName:"String",
    Phoneno:Bigint,
    Pass:"String",
    ConfirmPass:"String"
   }

## Response
  200-Success(OK)

Body (json) 
{ 
    Message:"SignUp Successful"
    user_id(userToken):Integer, 
    email:"String",
    username:"String",
    PhoneNo:Bigint,
    Password:"String",
    Time: "YYYY-MM-DD HH:mm:ss in Asia/Kolkata timezone"
}

404 - Not Found

400 - Bad Request 
     {
      Error:"error.details[0].message"
     }

500 - Internal Server Error
     {
      Error:"MySQL Query Error"
     }