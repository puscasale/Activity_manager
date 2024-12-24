# Activity_manager

## Overview

The **QT Activity Management System** is a sophisticated desktop application designed to help users effectively manage a variety of activities. Built using **C++** and the **Qt Framework**, this system offers a user-friendly graphical interface for adding, modifying, deleting, and filtering activities. It also includes advanced features such as basket management and activity reporting, making it an ideal solution for anyone who needs to organize and track activities with efficiency.

This application provides full CRUD (Create, Read, Update, Delete) functionality for activities, along with sorting, filtering, and advanced reporting capabilities. Furthermore, it supports an undo functionality to easily revert actions, making it both robust and user-friendly.

## Key Features

### Activity Management
- **Add Activities**: Users can input a new activity, specifying its name, description, type, and time. This is essential for maintaining a comprehensive list of activities.
- **Modify Activities**: Existing activities can be updated with new details, ensuring that the data is always current and accurate.
- **Delete Activities**: If an activity is no longer needed, users can easily remove it from the system.
  
### Filtering and Sorting
- **Filter Activities**: Activities can be filtered by description and type, enabling users to quickly find activities that match specific criteria.
- **Sort Activities**: The system allows activities to be sorted by name, description, type, or time, providing users with flexible viewing options.

### Activity Basket
- **Add to Basket**: Users can add selected activities to a basket for easier tracking or later review.
- **View Basket**: Users can view the activities currently in their basket and decide to clear or manage them.
  
### Activity Reporting
- **Generate Reports**: The application can generate detailed reports of all activities, categorizing them by type and offering insights into activity completion.
  
### Undo Functionality
- **Undo Actions**: If a mistake is made, users can easily undo the last modification, deletion, or addition, ensuring a smooth experience.

## Technologies and Tools Used

- **C++**: The core programming language used to develop the application.
- **Qt Framework**: Utilized to create the graphical user interface (GUI), ensuring a smooth and intuitive experience for the user.
- **Standard Template Library (STL)**: Leveraged for efficient data management and algorithmic operations.
- **C++11**: Features of C++11 such as unique pointers and references have been used for better memory management and performance.

## Application Architecture

The system is structured in a modular way to ensure maintainability, scalability, and ease of development:

1. **Activity Class** (`Activity.h`): Represents an activity with properties like name, description, type, and time.
2. **Repository** (`Repo.h`): Implements the data storage mechanism using an abstract repository interface (`RepoAbs`), with concrete implementations for in-memory storage (`Repo`), file-based storage (`RepoInFile`), and a lab-based storage system (`RepoLab`).
3. **Service Layer** (`Service.h`): Handles the core business logic of the application. It performs all operations like adding, modifying, and deleting activities, as well as managing the basket and generating reports.
4. **Undo Mechanism** (`Undo.h`): Implements the undo functionality, ensuring that users can easily revert the last action taken.
5. **Filtering Interface** (`Filter.h`): Graphical interface for applying filters to the list of activities, allowing users to find activities based on specific criteria.
6. **Dynamic Vector** (`DinamicVector.h`): A custom implementation of a dynamic vector to efficiently store and manage activities as the list grows.

## Installation Instructions

To get started with the QT Activity Management System, follow the instructions below:

### Prerequisites
Ensure you have the following installed:
- **Qt Framework**: The application is built using the Qt framework. You can download it from [Qt's official website](https://www.qt.io/download).
- **C++ Compiler**: A C++ compiler is required to compile the application (e.g., GCC, MSVC, Clang).
- **Qt Creator** (optional but recommended): Qt Creator is an integrated development environment (IDE) designed specifically for Qt applications. You can download it from [here](https://www.qt.io/qt-creator).

