## API for the Customer Visit the speicfic Hotel Home Page according to the hotel id with hotel details and visit track is save in database in    Hotel_Booking_and_Recommendation_System
   GET/api/HotelDetailsAndVisit/:id?UserID=?

## Request Headers
   Content-Type:application/json

#### Request params
     id:Int

#### Request query
     UserID=Int
   
## Response

  200-Success(OK)

Body (json) 
{ 
      "Message": "Customer Visit on hotel page",
      "HotelDetails":
        {
            "hotel_id": Int,
            "name": "String",
            "address": "String",
            "rating": Float,
            "price_per_night": Float,
            "discount": "String",
            "available": Boolean,
            "Area": "String",
            "City": "String",
            "State": "String",
            "Time": "YYYY-MM-DD HH:mm:ss in Asia/Kolkata timezone"
        }
}

404 - Not Found
     {
      Error:"Hotel not found"
     }

400 - Bad Request 
     {
      Error:"User ID is required"
     }

500 - Internal Server Error
     {
      Error:"MySQL Query Error"
     }