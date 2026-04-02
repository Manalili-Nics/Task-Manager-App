# Task Manager App 📱

A modern **Task Management Application** built with **Flutter** and **Firebase** that allows users to manage tasks with priority levels and due dates in real-time.

## ✨ Features

### 🔐 Authentication
- User registration with email/password
- Secure login/logout functionality
- Firebase Authentication integration

### 📝 Task Management (CRUD)
- ✅ Create new tasks
- 📖 Read tasks in real-time
- ✏️ Update existing tasks
- 🗑️ Delete tasks with confirmation

### 🎯 Bonus Features
- **Priority Levels** (Low/Medium/High) with color coding
  - 🔴 High Priority - Red
  - 🟠 Medium Priority - Orange  
  - 🟢 Low Priority - Green
- **Due Date Picker** - Set deadlines for tasks
- **Real-time Updates** - Changes appear instantly using StreamBuilder
- **Modern UI Design** - Gradient backgrounds, cards, and intuitive interface

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Flutter | Frontend mobile framework |
| Firebase Core | Firebase initialization |
| Firebase Auth | User authentication |
| Cloud Firestore | Real-time database |
| Dart | Programming language |

## 📱 Screenshots

|    Register     |     Login    |    Home   |
|-----------------|--------------|-----------|
| Register Screen | Login Screen | Task List |

|         Add Task         | Update Task |    Delete    |
|--------------------------|-------------|--------------|
| Add with priority & date | Edit dialog | Confirmation |

## 🏗️ Project Structure
lib/

├── main.dart # Main app entry point

├── RegisterScreen # User registration UI

├── LoginScreen # User login UI

├── HomeScreen # Task management UI

└── AuthService # Authentication logic


## 🗄️ Firestore Database Structure
tasks 

└── {documentId}

├── title: String

├── priority: String (low/medium/high)

├── dueDate: Timestamp (optional)

├── createdAt: Timestamp

└── userId: String (links to authenticated user)




## 🚀 Getting Started

Prerequisites

Flutter SDK installed
Android Studio / VS Code
Firebase account

Installation
Clone the repository

git clone https://github.com/Manalili-Nics/Task-Manager-App.git
cd Task-Manager-App

Install dependencies
flutter pub get

Run the app
flutter run -d chrome

Firebase Setup

Create a Firebase project at Firebase Console
Register a web app in your Firebase project
Copy your Firebase configuration
Update the FirebaseOptions in lib/main.dart with your config:
await Firebase.initializeApp(
  options: const FirebaseOptions(
    apiKey: "YOUR_API_KEY",
    authDomain: "YOUR_AUTH_DOMAIN",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_STORAGE_BUCKET",
    messagingSenderId: "YOUR_SENDER_ID",
    appId: "YOUR_APP_ID",
  ),
);

Enable Email/Password Authentication in Firebase Console
Create Firestore Database in test mode

## 📋 Usage Guide

Register a new account with email and password
Login with your credentials
Add a task by clicking the + button
Enter task title
Select priority (Low/Medium/High)
Choose due date (optional)
Edit a task by clicking the blue edit icon
Delete a task by clicking the red delete icon
Logout using the logout button in the app bar

## 🎯 Learning Outcomes

After completing this lab activity, students should be able to:
Connect a Flutter app to Firebase
Implement Firebase Authentication (Email & Password)
Perform CRUD operations using Cloud Firestore
Use StreamBuilder for real-time updates
Apply basic Firebase security rules
Build a professional mobile UI with Flutter

Troubleshooting

|         Error	       |                      Solution                     |
|----------------------|---------------------------------------------------|
|api-key-not-valid	   | Copy exact API key from Firebase Console          |
|Registration failed	 | Ensure Email/Password is enabled in Firebase Auth |
|Firestore not working | Create Firestore database in test mode first      |
|StreamBuilder error	 | Check userId field matches authenticated user     |


## Author
Nicole Manalili

GitHub: @Manalili-Nics

Email: manalilinicole33@gmail.com


## 🎓 Course
Advanced Mobile Development - Laboratory Activity 6

Flutter + Firebase Task Manager App

Week 9–10 Laboratory Activity


## 📄 License
This project is created for educational purposes as part of a laboratory activity.


## 🙏 Acknowledgments
Flutter Documentation

Firebase Documentation

Course Instructor

