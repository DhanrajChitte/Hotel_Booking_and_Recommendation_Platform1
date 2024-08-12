## API for the Book the Hotel from the Hotel Home Page if the Customer Pay the Amount then Booking Completed Otherwise Draft Booking in Hotel_Booking_and_Recommendation_System
   POST/api/booking

## Request Headers
   Content-Type:application/json

#### Request body
   {
    "User_id": Int,
    "Hotel_id": Int,
    "NoOFNights": Int,
    "NoOFPeople": Int,
    "check_in_time": "YYYY-MM-DD HH:mm:ss in Asia/Kolkata timezone",
    "check_out_time": "YYYY-MM-DD HH:mm:ss in Asia/Kolkata timezone",
    "Payment_Status": "completed/draft"
   }
   

## Response
  201-Success(Created)

Body (json) 
{
        Message: `Booking ${Booking_Status} successfully`,
        Booking_ID: result.insertId,
        Booking_Status: Booking_Status,
}

404 - Not Found

400 - Bad Request 
     {
      Error:"error.details[0].message"
     }

500 - Internal Server Error
     {
      Error:"Internal Server Error"
      Error:"MySQL Query Error"
     }