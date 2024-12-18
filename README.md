# APIs


## /mockEvents.json
This API contains a list of 100 event objects, each with unique details, structured as follows:

- **ID**: A unique identifier for each event.
- **Title**: A title relevant to the event's category.
- **Time**: Date and time of the event in UTC format, ensuring no past events.
- **Location**: A city and country location for the event.
- **Description**: A brief, category-specific description of the event, using simple language.
- **LongDescription** A longer version of the description to replace any _Lorem Ipsum_ text.
- **Image**: A placeholder URL (`https://via.placeholder.com/350x200`) used for all events.
- **Price**: A randomly assigned price (e.g., £10, £50) or marked as "Free."
- **Category**: Each event is categorized under one of six themes:
  - Technology
  - Art & Design
  - Music
  - Food & Drink
  - Fashion
  - Sports

This format helps maintain consistency and relevance across events, making it suitable for use in an events database or similar application.

## /mockWeather.json

This API contains a list of city weather objects, each with detailed weather information, structured as follows:

- **City**: The name of the city where the weather data is applicable.
- **Country**: The name of the country where the city is located.
- **WeatherData**: A nested object containing specific weather information:
- **Temperature**: A floating-point number representing the current temperature in Celsius (e.g., 23.5).
- **Description**: A brief description of the current weather conditions (e.g., "Clear sky", "Cloudy").
- **Icon**: A string representing the weather condition code, following the OpenWeather icon format (e.g., "01d", "03d").

### How to Use the Data
Each city's weather data includes an icon code that follows the OpenWeather standards. You can use this icon code to display weather icons by constructing a URL like this:
```
https://openweathermap.org/img/wn/{icon_code}@2x.png
```
For a city with an icon code 01d (representing a clear sky during the day), the corresponding image URL would be:
```
https://openweathermap.org/img/wn/01d@2x.png
```
This link will show an image of the current weather based on the icon code.

You can use the weather data and icons to display weather conditions in any app or website.
