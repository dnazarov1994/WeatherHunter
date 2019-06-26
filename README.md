# Weather Hunter
The Weather Hunter app allows the user to see current weather **anywhere in the World** just by tapping a map! You don't need to know exactly the name of the city or town! This app is very helpful for your road trip or family vacation in the new location!

## Architecture
The app has two view controller scenes:
- Map View
- Table View

## App Functionality 
When the user opens the Weather Hunter app, the Map View appears. The user is able to zoom and scroll around the map using standard pinch and drag gestures. Tapping and holding the map drops a new pin. Users can place any number of pins on the map. When the user placed a pin, the "SEE WEATHER" button is enabled. By tapping this button the Table View controller appears. While the data is downloading, the Table View in a temporary “downloading” state. In this View Controller user can see the location name (if it exists), current temperature in Fahrenheit and logo with current weather conditions associated with the latitude and longitude of the pin. The weather information is displayed in the same sequence as the pins were placed on the Map. By selecting a pin on the map, the "DELETE PIN" button is enabled. By tapping this button, the pin is removing from the app. All pins are saved in the same locations after reopening the app.

## Data from network resources
The Weather Hunter app using data from the OpenWeatherMap API: "https://api.openweathermap.org/data"

## Error handling
If the submission fails to post the data to the server, then the user sees an alert with an error message describing the failure. 

### Requirements

Xcode 9.2
Swift 4.0

