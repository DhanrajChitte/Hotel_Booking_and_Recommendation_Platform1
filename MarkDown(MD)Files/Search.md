## Hotels Search API according to the hotel name,area,city,state,price & rating for  Customer in Hotel_Booking_and_Recommendation_System
   GET/api/SearchHotels

## Request Headers
   Content-Type:application/json

#### Request params
   
    Name:"String",
    Area:"String",
    City:"String",
    State:"String"
    Rating:Int/Float,
    Price:Int/Float
   

## Response
  200-Success(OK)

Body (json) 
{
    "Hotels": 
    [
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
    ]
}

404 - Not Found

400 - Bad Request 
     {
      Error:"Search for the that hotels whose name,area,city,state,price,rating, not match "
     }

500 - Internal Server Error
     {
      Error:"An error occurred while searching for hotels"
      Error:"MySQL Query Error"
     }