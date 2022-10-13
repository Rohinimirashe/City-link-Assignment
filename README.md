# City-link-Assignment
Modules


Create POST request REST API. The API should expect input payload as mentioned in the URL: https://clstorageapp.blob.core.windows.net/assignment/booking.json and do the following:
Parse the data and insert it into the database. Database can be MongoDB or MySQL.
Create two tables, one for user and other for booking info based on fields available in URL
User Table: userId, fullName, mobile, email
Booking Table: bookingId, bookingTime, pickupTime, sourceName, sourceAddress, sourceLocation, sourceCity, sourceState, sourcePostalCode, sourceCountry, sourceLatitude, sourceLongitude, destinationName, destinationAddress, destinationLocation, destinationCity, destinationState, destinationPostalCode, destinationCountry, destinationLatitude, destinationLongitude
Vendor Table: vendorId, driverName, vehicleNumber, vehicleMake, vehicleModel
Store the parsed data in the tables
 

You can choose Node.js / Express.js to develop these API’s and this assign

Install the dependencies and devDependencies and start the server.

$ npm i express
$ npm i mongoose
$ npm install -d
 Postman code -
 {
	"context": "Trucking",
	"type": "Booking",
	"bookingId": "78500",
	"source1": "MobileApp",
	"status": "Confirmed",
	"customer": {
	
		"fullName": "John Doe",
		"mobile":  "+91 9980798456",
		"email":"john_doe@gmail.com"
	},
	"source": {
		"name": "AMC Mercado",
		"address": {
			"address": "1858, 2821, Mission College Road",
			"location": "Koramangala",
			"city": "Bangalore",
			"state": "Karnataka",
			"postalCode": "560034",
			"country": "India"
		},
		"latitude":"12.933664",
		"longitude":"77.616179"
	},
	"destination": {
		"name": "Jayem Logistics",
		"address": {
			"address": "#7, Road Number 10, KIADB",
			"location": "Whitefileld",
			"city": "Bangalore",
			"state": "Karnataka",
			"postalCode": "560066",
			"country": "India",
			"coordinates": {
				"latitude":"12.984955",
				"longitude":"77.727345"
			}
		}
	},
	"vendor": {

		"fullName": "Ram",
		"vehicleNumber": "KA01AB9876",
		"vehicleModel": "Tata Ace"
	},
	"bookingTime": "2020-08-31T11:15:22-06:00",
	"pickupTime": "2020-08-31T15:00:00-00:00"
}

And run the application in the development mode.
