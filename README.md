Task Manager App

Overview

The Task Manager App is an Android application that helps users manage their daily tasks efficiently. It allows users to create, update, and delete tasks while also tracking their completion status. The app integrates with a cloud-based backend (Firebase Firestore) to store tasks persistently, enabling users to access their tasks from multiple devices.

Key Features

Add New Tasks – Users can create new tasks with a title and completion status.

Mark Tasks as Completed – Tasks can be marked as completed or pending via a checkbox.

Delete Tasks – Swipe-to-delete functionality for removing tasks from the list.

Cloud Storage – Tasks are stored in Firebase Firestore to enable persistent access.

Network Communication – The app fetches and updates data using Firebase's web-based API.

User-Friendly Interface – Simple and intuitive UI with RecyclerView for managing tasks.

Software Components

MainActivity.java – Handles the main UI, displaying tasks and integrating the RecyclerView.

TaskAdapter.java – Manages task list rendering, updates, and swipe-to-delete interactions.

Task.java – Data model representing each task (title, completion status, ID).

Firebase Firestore – Cloud database for storing tasks.

Layouts:

activity_main.xml – UI for displaying the task list.

item_task.xml – Layout for individual task items.

dialog_add_task.xml – Input dialog for adding tasks.

Wireframes & Class Diagram

(Include wireframe and class diagram images here in the final submission.)

Web Service Used

The app communicates with Firebase Firestore via its RESTful API for CRUD operations on tasks.

Web Service URL: https://firestore.googleapis.com/v1/projects/{project-id}/databases/(default)/documents/tasks

Operations:

GET – Retrieve tasks

POST – Add a new task

PATCH – Update a task

DELETE – Remove a task

How to Run the Project

Clone the Git repository.

Open the project in Android Studio 4.0.1.

Connect Firebase Firestore and update google-services.json.

Compile and run on an emulator or physical device (Android 5.1 Lollipop, API 22).
