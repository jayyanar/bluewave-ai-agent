Bluewave Holidays Travel AI Agent - README
Welcome to the Bluewave Holidays Travel AI Agent project, focusing on planning luxury vacations in the Maldives. This guide will walk you through the setup and usage of an AI-powered Booking Assistant using Amazon Bedrock Agents.

Agent Overview
Our AI Booking Assistant helps you plan your dream vacation in the Maldives. 🌴 Dive into vibrant marine life, sail towards fiery sunsets, and bask in paradise. Ready for an unforgettable getaway? Let's get started!

Agent Architecture Diagram

What the Booking Assistant Can Do
Get Latest Booking Updates
Pull the latest updates for your bookings. The booking name doesn't need to be an exact match, as our orchestration Lambda function handles name-to-id conversion.

Example:

text
Copy code
"Get updates on my BluewaveHolidays booking."
Translate Booking Details
Translate booking details to English if they are in another language.

Example:

text
Copy code
"Translate the latest booking details from BluewaveHolidays."
Summarize Booking Information
Summarize booking information from a specific reservation. If details are in another language, they will be translated to English before summarization.

Example:

text
Copy code
"Summarize my BluewaveHolidays booking."
Query Bookings Based on a Custom Prompt
Ask specific questions about your bookings. If details are in another language, they will be translated to English before querying.

Example:

text
Copy code
"What are the top resort recommendations for my BluewaveHolidays booking?"
What is Bedrock Agent?
Agents for Amazon Bedrock help accelerate generative AI application development by orchestrating multistep tasks. They can make different API calls, understand user requests, break down complex tasks into multiple steps, collect additional information, and take actions to fulfill requests.

AWS News Blog: Enable Foundation Models to Complete Tasks With Agents for Amazon Bedrock
AWS News Blog: Agents for Amazon Bedrock is now available with improved control of orchestration and visibility into reasoning
