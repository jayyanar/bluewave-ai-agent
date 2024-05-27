# Bluewave Holidays Travel AI Agent
Welcome to the Bluewave Holidays Travel AI Agent project, focusing on planning luxury vacations in the Maldives. This guide will walk you through the setup and usage of an AI-powered Booking Assistant using Amazon Bedrock Agents.

## Agent Overview
Our AI Booking Assistant helps you plan your dream vacation in the Maldives. 🌴 Dive into vibrant marine life, sail towards fiery sunsets, and bask in paradise. Ready for an unforgettable getaway? Let's get started!


## What is Bedrock Agent?
Agents for Amazon Bedrock help accelerate generative AI application development by orchestrating multistep tasks. They can make different API calls, understand user requests, break down complex tasks into multiple steps, collect additional information, and take actions to fulfill requests.



## OpenAPI Schema Endpoints with Descriptions

### 1 /plan-vacation

POST: Plan a Maldives luxury vacation based on the provided budget and preferences.
Description: Takes the user's budget, preferences (e.g., overwater villa, spa, diving, private beach), start date, and end date to plan a vacation, generating an itinerary ID.

### 2 /generate-itinerary

GET: Generate a detailed itinerary for a Maldives vacation using the provided itinerary ID.
Description: Retrieves and generates a detailed itinerary of the vacation based on the provided itinerary ID.

### 3 /send-itinerary

POST: Send the generated itinerary via email or SMS.
Description: Sends the itinerary, identified by its ID, to the specified email address or phone number via the chosen method (email or SMS).

### 4 /available-resorts

GET: Get available luxury resorts in the Maldives based on user preferences.
Description: Retrieves a list of luxury resorts in the Maldives that match the user's specified preferences.

### 5 /book-accommodation

POST: Book luxury accommodation in the Maldives based on the itinerary ID and accommodation details.
Description: Books accommodation using the provided itinerary ID and details such as accommodation name, address, check-in date, and check-out date.

### 6 /review-itinerary

GET: Review the details of the Maldives vacation itinerary based on the itinerary ID.
Description: Allows users to review the detailed itinerary of their Maldives vacation using the provided itinerary ID.
This schema focuses on providing a comprehensive and luxurious vacation planning experience in the Maldives through Bluewave Holidays' AI travel assistant.

