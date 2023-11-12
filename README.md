# Welcome to Awesome AI Accelerators! 🤖🦾

## AI Recognition Accelerator with Node.js and ml5.js

This accelerator template leverages the simplicity and efficiency of Node.js and Express to create an AI Recognition Accelerator, featuring real-time object detection using ml5.js. It provides a user-friendly interface built with Materialize CSS, enabling dynamic interaction with AI models.

## Key Features

- **Real-Time Object Detection**: Utilizes ml5.js to process video streams in real-time, identifying and classifying objects efficiently.
- **User-Friendly Interface**: A sleek UI powered by Materialize CSS, providing an intuitive experience for users to interact with the AI model.
- **Customizable Settings**: Options to toggle AI functionalities and adjust frame rate (FPS) for the video stream.

## Getting Started

To run this app, you'll need a basic setup with Node.js and npm installed. Clone the repository and install dependencies:

```shell
git clone [your-repo-link]
cd [your-repo-directory]
npm install
```

## Then, start the server with:

```shell
npm start
```
The app will be available at http://localhost:80.

## Deploying on VMware Tanzu Application Platform
To deploy this application on VMware Tanzu Application Platform, follow these steps:

Ensure you have the Tanzu CLI installed and configured with access to your Tanzu Application Platform instance.

### Navigate to your project directory:

```shell
cd [your-repo-directory]
```
### Use the Tanzu CLI to deploy your application:

```shell
tanzu apps workload create -f config/workload.yaml
```

### Monitor the deployment status:

```shell
tanzu apps workload tail ai-video-recognition --timestamp --since 1h
```

Once deployed, access your application via the URL provided by Tanzu Application Platform. You can find the url with the following command:

```shell
tanzu apps workload get ai-video-recognition
```

## Overview
The index.html of this app contains:

- A video element for real-time video streaming.
- A canvas to display the processed video.
- Controls for toggling AI processing and adjusting FPS.
- Integration of ml5.js for object detection functionalities.

## How to Contribute
Contributions to improve or enhance this AI Recognition Accelerator are welcome. Feel free to open issues or submit pull requests with your suggestions or improvements.

## Please Note
The software is provided "as is", without warranties of any kind. As the creator, I am not liable for any claims, damages, or other liabilities that arise from the use of the work.


