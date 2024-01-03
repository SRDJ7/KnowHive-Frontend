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

### Frontend Hosting ###
Our React frontend is hosted on Apache2, a web server, making it accessible to users at `https://knowhive.centralindia.cloudapp.azure.com/`. The deployment involves placing our React files in a designated directory on an Azure Virtual Machine with the following specifications:
* Operating System: Linux (Ubuntu 22.04)
* Size: Standard D2as v4 (2 vCPUs, 8 GiB memory)
* Disk Storage: Premium SSD LRS (30 GiB)

Apache's Virtual Host is set up to point to the React files on this VM, allowing users to access our React app seamlessly.

Let's Encrypt SSL Certificates, obtained through Certbot, enhance security by automating SSL protection for communication between users and Apache2. These certificates automatically renew, ensuring uninterrupted SSL security.

Apache2 serves as a reverse proxy for our backend (Flask API), forwarding user requests while handling SSL encryption. Users securely access our application via HTTPS, while Apache2 communicates with the backend using regular HTTP, simplifying SSL complexities.

Additionally, Apache2 automatically redirects HTTP requests to HTTPS, seamlessly directing users to the secure version of our application at `https://knowhive.centralindia.cloudapp.azure.com/`. This contributes to an overall safer browsing experience on our Azure VM-hosted React frontend.

## Glimpse of KnowHive UI ##

<p align="center">
<img width="960" alt="Start Page" src="https://github.com/SRDJ7/KnowHive-Frontend/assets/67571677/ecfc65ab-dcb0-469e-be02-995900ebdc83">
Display of Start Page
</p>


<p align="center">
<img width="960" alt="Signup Page" src="https://github.com/SRDJ7/KnowHive-Frontend/assets/67571677/19055004-a0df-4054-8bae-9476271655c5">
Display of Signup Page
</p>

<p align="center">
<img width="960" alt="Login Page" src="https://github.com/SRDJ7/KnowHive-Frontend/assets/67571677/408d0deb-2c69-49c4-9f0e-b4ad85e2d3b8">
Display of Login Page
</p>

<p align="center">
<img width="960" alt="Chat Page" src="https://github.com/SRDJ7/KnowHive-Frontend/assets/67571677/09bbcea5-f1c5-4b32-98bf-68d2a67088e2">
Display of Chat Page
</p>

<p align="center">
<img width="960" alt="chat page with response from GPT Model" src="https://github.com/SRDJ7/KnowHive-Frontend/assets/67571677/65860cf3-a962-488c-b43f-249cfa5a2cc3">
Display of chat page with response from GPT Model
</p>

<p align="center">
<img width="960" alt="Chat Modal" src="https://github.com/SRDJ7/KnowHive-Frontend/assets/67571677/21e23f48-f554-4b9e-aca8-1a290e2f66c9">
Display of Chat Modal
</p>

<p align="center">
<img width="960" alt="Video Modal" src="https://github.com/SRDJ7/KnowHive-Frontend/assets/67571677/e37f3677-4cac-47c9-8576-abbe3bb990bf">
Display of Video Modal
</p>
