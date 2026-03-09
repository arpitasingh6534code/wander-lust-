
# Wanderlust Web Project – Installation Guide

This document explains how to set up and run the **Wanderlust web application** on your local machine. Follow the instructions carefully to install all required dependencies and start the project.

---

## Requirements

Make sure the following software is installed on your system before starting:

- **Node.js** (Recommended version: 18 or above)
- **MongoDB**
- **Nodemon** (install globally)

To install Nodemon globally:

```
npm install -g nodemon
```

---

## Step 1: Clone the Repository

Download the project from GitHub using the following command:

```
git clone https://github.com/arpitasingh6534code/wander-lust-
```

After cloning, move into the project folder:

```
cd wander-lust-
```

---

## Step 2: Configure Environment Variables

Create a file named **.env** in the root folder of the project.

Add the following MongoDB connection string:

```
ATLASDB_URL=mongodb://127.0.0.1:27017/wanderlust
```

This will connect the project to your local MongoDB database.

---

## Step 3: Configure Cloudinary

Cloudinary is used in this project to upload and manage images.

1. Visit https://cloudinary.com
2. Create a free account and log in.
3. From the dashboard, copy the following credentials:
   - Cloud Name
   - API Key
   - API Secret

Add them to your **.env** file:

```
CLOUD_NAME=your_cloud_name
CLOUD_API_KEY=your_api_key
CLOUD_API_SECRET=your_api_secret
```

---

## Step 4: Add Application Secret

For authentication and session security, add a secret key in the **.env** file.

```
SECRET=your_secure_secret_key
```

You can choose any random secure value.

---

## Step 5: Install Project Dependencies

Install all required packages using npm:

```
npm install
```

---

## Step 6: Start the Application

Run the project using Nodemon:

```
nodemon app.js
```

Nodemon will automatically restart the server whenever you make changes to the code.

---

## Step 7: Open the Application

Once the server starts successfully, open your browser and visit:

```
http://localhost:8080
```

You should now see the **Wanderlust web application** running locally.

---

## Project Setup Complete 🎉

You have successfully installed and configured the Wanderlust project on your system. If you face any issues during setup, check your environment variables and database connection.
