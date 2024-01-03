# KnowHive-Frontend
Welcome to the KnowHive repository! This React-based frontend application allows field engineers seeking quick access to accurate and up-to-date knowledge for resolving incidents efficiently and effectively. This web application has been specifically designed to empower field engineers with an intelligent chatbot interface, providing instant assistance and valuable insights to tackle diverse challenges encountered in the field.

## Key Features ##
*  __Real-time Chat:__ Engage in instantaneous conversations with the intelligent KnowHive assistant.
*  __Voice Input:__ Leverage voice recognition to swiftly input questions and receive prompt responses.
*  __Narration Option:__ Explore the speaker option, enabling the KnowHive assistant to narrate responses for enhanced accessibility.
*  __Chat History:__ Keep track of your interactions with the KnowHive assistant, providing a valuable reference for future problem-solving.
*  __Video Demo:__ Access a video demonstration to gain a comprehensive understanding of the KnowHive's capabilities.

## Tech Stack ##
*  __Framework:__ React.js
*  __Hosting:__ Azure Virtual Machine
*  __Web Server:__ Apache2 (SSL termination via Let's Encrypt).
*  __SSL Certificate:__ Let's Encrypt.

## Getting Started ##
To run the KnowHive assistant Application locally, follow these steps:
1. Clone the repository:
`git clone`

2. Navigate to the project directory:
`cd knowhive-chat-app`

3. Install dependencies:
`npm install`

4. Start the development server:
`npm start`

### Configuration ###
Make sure to configure the backend server URL in the axios requests within the code. Update the URL accordingly in the following pages:

* __SignUpPage.js__ : http://127.0.0.1:5000/signup
* __LoginPage.js__ : http://127.0.0.1:5000/login
* __ChatPage.js__ : http://127.0.0.1:5000/ask
* __ChatHistoryModal.js__ : http://127.0.0.1:5000/conversation-history

This will launch the application locally. Open your browser and go to `http://localhost:3000` to interact with the KnowHive assistant.

#### KnowHive Backend Github repository ####
To access the KnowHive backend code [Click Here](https://github.com/SRDJ7/KnowHive-Backend)

## Glimpse of KnowHive UI ##
