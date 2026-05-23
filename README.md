# Room MVVM Demo

A simple Android application that demonstrates the implementation of **Room Persistence Library** using the **MVVM (Model-View-ViewModel) architecture**.

## Features
- **Add Notes**: Create new notes with a title, description, and priority.
- **Delete Notes**: Swipe or click to remove individual notes.
- **Delete All**: Clear the entire database.
- **Data Persistence**: Uses Room to store notes locally in a SQLite database.
- **Reactive UI**: Utilizes `LiveData` to automatically update the UI when data changes.
- **Lifecycle Awareness**: Uses `ViewModel` to manage data across configuration changes.

## Architecture
The project follows the official Android architectural recommendations:
- **Entity**: Defines the schema of the database table (`Note`).
- **DAO**: Provides methods for accessing the database (`NoteDao`).
- **Room Database**: The main access point to the underlying SQLite database.
- **Repository**: A clean API for data access, abstracting the data source from the ViewModel.
- **ViewModel**: Provides data to the UI and survives configuration changes.
- **UI (Activity & Adapter)**: Displays the data to the user using `RecyclerView`.

## Tech Stack
- **Language**: Java
- **Database**: [Room](https://developer.android.com/training/data-storage/room)
- **Architecture**: MVVM
- **Components**: LiveData, ViewModel, RecyclerView, CardView
- **UI Design**: Material Design

## Project Structure
- `data/local`: Contains Room configuration (Entity, DAO, Database).
- `data`: Contains the Repository class.
- `viewmodel`: Contains the ViewModel managing the UI data.
- `ui`: Contains the Activity and RecyclerView Adapter.

## Getting Started
1. Clone the repository.
2. Open the project in Android Studio.
3. Build and run the app on an emulator or physical device.
