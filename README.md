# Bluewave Holidays Travel AI Agent
Welcome to the Bluewave Holidays Travel AI Agent project, focusing on planning luxury vacations in the Maldives. This guide will walk you through the setup and usage of an AI-powered Booking Assistant using Amazon Bedrock Agents.

## AI  Agent Overview
Our AI Booking Assistant helps you plan your dream vacation in the Maldives. 🌴 Dive into vibrant marine life, sail towards fiery sunsets, and bask in paradise. Ready for an unforgettable getaway? Let's get started!


# Improved efficiency in Travel Customer Service using Amazon Q's  

![Screenshot 2024-05-27 at 3 40 50 PM](https://github.com/jayyanar/bluewave-ai-agent/assets/12956021/5d8563e1-b178-41ee-97df-41932a9e2a8f)


## Detailed Information on Youtube: https://youtu.be/FGaIxlvWVhw - Step by Step Instruction.


### 1\. Developer Setup and Deployment

*   **GitHub Repository:**
    
    *   Developers maintain the source code in a GitHub repository.
        
    *   They use Amplify CLI to manage and deploy the application.
        
*   **Amplify CLI:**
    
    *   The CLI tool is used to initialize, configure, and deploy AWS Amplify projects.
        
    *   Code changes pushed to GitHub can trigger CI/CD pipelines (if set up), deploying changes to AWS Amplify.
        

### 2\. Frontend - AWS Cloud

*   **Amplify Web Hosting:**
    
    *   The application’s frontend is hosted using AWS Amplify Hosting, which provides a scalable web hosting solution.
        
    *   Developers deploy the frontend code to Amplify Hosting directly from the CLI or CI/CD pipelines.
        
*   **Amazon Cognito for Authentication:**
    
    *   Cognito handles user authentication and authorization, allowing secure access to the application.
        
    *   Resort managers log in via the UI at **https://portal.bluewaveholiday.net** using credentials managed by Cognito.
        
*   **Route 53:**
    
    *   AWS Route 53 manages DNS and provides a custom domain for the application, ensuring users can access the site via **https://portal.bluewaveholiday.net**.
        

### 3\. Data Sources and Storage

*   **Amazon S3:**
    
    *   Stores PDFs, XLSX files, websites, and other datasources.
        
    *   These files can be uploaded and accessed as needed by different parts of the application.
        

### 4\. Backend Processing

*   **AWS Lambda:**
    
    *   Used for event-driven processing.
        
    *   Automatically triggers to refresh data for Amazon Q (possibly through data ingestion, transformation, or updating search indices).
        
    *   Ensures that the data presented in the application is up-to-date.
        

### 5\. Generative AI with Amazon Q

*   **Amazon Q:**
    
    *   Serves as the generative AI engine for processing and analyzing data.
        
    *   It utilizes the data from Amazon S3 and other integrated datasources to provide intelligent insights or responses.
        
*   **IAM Center for IDP:**
    
    *   Manages identities and permissions for accessing Amazon Q.
        
    *   Ensures secure access to the AI functionalities, only allowing authorized personnel or services to interact with the AI.
        

### 6\. User Interaction - Travel Agents

*   **Chat UI from Amazon Q:**
    
    *   Travel agents interact with the system via a chat interface at **https://chat.bluewaveholiday.net**.
        
    *   This chat UI is powered by Amazon Q, providing generative AI-driven responses and assistance to the travel agents.
        

### Workflow Summary:

1.  **Code Deployment:** Developers push code to GitHub and deploy using Amplify CLI.
    
2.  **Frontend Hosting:** Amplify Web Hosting serves the frontend application, secured with Cognito authentication.
    
3.  **Data Storage:** Data such as PDFs and Excel files are stored in Amazon S3.
    
4.  **Data Processing:** AWS Lambda functions handle event-driven updates to ensure fresh data.
    
5.  **AI Integration:** Amazon Q processes and analyzes data, utilizing IAM for secure access.
    
6.  **User Interaction:** Travel agents use the chat UI powered by Amazon Q for their operations.
    

This workflow ensures a streamlined process from development to deployment, with secure access, efficient data processing, and intelligent AI-driven interactions.







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

