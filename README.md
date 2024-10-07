# EventsAPI


/mockEvents.json
This API contains a list of 100 event objects, each with unique details, structured as follows:

- **ID**: A unique identifier for each event.
- **Title**: A title relevant to the event's category.
- **Time**: Date and time of the event in UTC format, ensuring no past events.
- **Location**: A city and country location for the event.
- **Description**: A brief, category-specific description of the event, using simple language.
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
