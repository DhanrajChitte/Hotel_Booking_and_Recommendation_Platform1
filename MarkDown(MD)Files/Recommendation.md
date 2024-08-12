## API for the Recommendation of the New Hotels List for the Customer based on his visits records and draft/completed booking on various criteria such as area,city,state,rating,price of the previous hotels in Hotel_Booking_and_Recommendation_System
   GET/api/recommendations/:User_id

## Request Headers
   Content-Type:application/json

#### Request params
    "User_id":Int   

## Response
  200-Success(OK)

Body (json) 
{ 
    "Message": "Recommended hotels fetched successfully",
    "Message": "No past visits or bookings found",
    "Recommendations":
    [
        {
            "hotel_id": Int,
            "hotel_name": "String",
            "address": "String",
            "rating": Float,
            "price_per_night": Float,
            "discount": "String",
            "available": Boolean,
            "Area": "String",
            "City": "String",
            "State": "String"
        }
    ]
}

404 - Not Found

400 - Bad Request 
     {
      Error:"Invalid User ID"
     }

500 - Internal Server Error
     {
      Error:"Internal Server Error"
      Error:"MySQL Query Error"
     }