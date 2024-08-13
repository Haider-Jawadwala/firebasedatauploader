# Firebase Data Upload Tool

This simple web application allows users to upload JSON data to a Firebase Firestore database. It provides a user-friendly interface with a progress bar to monitor the upload process.

## Features

- Upload JSON files to Firebase Firestore
- Real-time progress tracking
- Simple and intuitive user interface

## Prerequisites

Before you begin, ensure you have the following:

1. A Firebase account and a Firebase project set up
2. Basic knowledge of HTML, JavaScript, and Firebase

## Setup

1. Clone this repository to your local machine:
```
git clone https://github.com/Haider-Jawadwala/firebasedatauploader.git
```

2. Navigate to the project directory:
```
cd firebase-data-upload
```

3. Open the `index.html` file in a text editor.

4. Replace the `firebaseConfig` object with your own Firebase configuration:
```javascript
const firebaseConfig = {
    apiKey: "YOUR_API_KEY",
    authDomain: "YOUR_AUTH_DOMAIN",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_STORAGE_BUCKET",
    messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
    appId: "YOUR_APP_ID",
    measurementId: "YOUR_MEASUREMENT_ID"
};
```
## Usage

1. Open the `index.html` file in a web browser.

2. Click on the "Choose File" button and select a JSON file containing the data you want to upload.

3. Click the "Upload Data" button to start the upload process.

4. The progress bar will show the upload status, and you'll see a message indicating how many documents have been uploaded.
   
## JSON File Format

The JSON file should have the following structure:

```json
{
  "collectionName": [
    {
      "field1": "value1",
      "field2": "value2"
    },
    {
      "field1": "value3",
      "field2": "value4"
    }
  ]
}
```

## Example
```
{
  "products": [
    {
      "name": "Widget A",
      "price": 9.99,
      "inStock": true
    },
    {
      "name": "Gadget B",
      "price": 19.99,
      "inStock": false
    }
  ]
}
```

## Troubleshooting

If you encounter CORS issues, you may need to set up Firebase Hosting or use a local server to run the application.
Make sure your Firebase project has the necessary permissions set up for reading and writing to Firestore.




