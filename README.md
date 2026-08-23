# DaanPH

### Offline Public Transportation and Commuter Navigation for the Philippines

**DaanPH** is an offline-first commuter navigation application designed to help Filipinos discover and navigate public transportation routes across the Philippines, even without an internet connection.

DaanPH stores essential transportation, geographic, and map data locally on the device, allowing core search and routing functionality to operate offline.

> DaanPH — Find your way, even offline.

---

## Overview

Navigating public transportation in the Philippines can be difficult, especially when traveling through unfamiliar areas or when internet connectivity is limited.

DaanPH aims to simplify this process by providing a centralized offline commuter tool for finding routes, transportation stops, destinations, and estimated fares.

The application is designed specifically around the structure and challenges of Philippine public transportation.

---

## Features

### Offline Maps

DaanPH supports locally stored map data so users can access essential map information without continuously relying on an internet connection.

### Public Transportation Routing

The application searches available transportation data to determine possible routes between an origin and destination.

The routing system can account for multiple transportation services and transfers.

### Fare Estimation

DaanPH provides estimated fares for supported transportation routes based on Philippine public transportation fare data.

### Offline Place Search

Users can search for destinations, landmarks, transportation stops, and other locations using locally stored data.

### Origin and Destination Search

Users can select an origin and destination and receive possible commuting routes between them.

### Offline-First Architecture

Core functionality is designed to operate locally rather than requiring every request to be sent to a remote backend.

Essential transportation and geographic data can be bundled directly with the application.

---

## How It Works

The general routing pipeline works as follows:

```text
User
 |
 v
Search Origin and Destination
 |
 v
Local Place Search
 |
 v
Find Nearby Transportation Stops
 |
 v
Route Search Engine
 |
 v
Transfer and Path Exploration
 |
 v
Fare Calculation
 |
 v
Route Instructions
 |
 v
Offline Map Visualization
```

DaanPH performs route discovery using locally available transportation data, allowing core functionality to remain available without an active internet connection.

---

## Technology Stack

### Mobile Application

* Flutter
* Dart
* Flutter Map
* latlong2

### Local Database

* SQLite
* sqflite
* FTS5 Full-Text Search
* Bundled offline database

### Geographic and Transportation Data

* OpenStreetMap data
* Offline map tiles
* Philippine transportation datasets
* Geographic and place data

### Development Tools

* Git
* GitHub
* Python
* SQLite
* Flutter tooling

---

## Offline Data Pipeline

DaanPH uses a data-processing pipeline to transform transportation and geographic datasets into an application-ready SQLite database.

```text
Raw Transportation and Geographic Data
                  |
                  v
          Data Extraction
                  |
                  v
          Data Processing
                  |
                  v
          SQLite Database
                  |
                  v
       Flutter Offline Application
                  |
                  v
      Search, Routing, and Mapping
```

The project includes tools for processing and generating the offline database used by the application.

---

## Built for the Philippines

DaanPH is specifically designed for Philippine transportation.

Depending on available data, the application can work with information relating to:

* Jeepneys
* Buses
* Rail transportation
* Public transportation stops
* Transit routes
* Roads
* Places and landmarks

The long-term goal is to expand transportation coverage and improve route accuracy across more areas of the Philippines.

---

## Why Offline?

Many navigation applications depend heavily on:

* Internet connectivity
* Remote APIs
* Online map services
* Real-time backend services

DaanPH takes an offline-first approach for its core functionality.

By keeping important transportation and geographic data locally available, the application can continue providing essential commuter functionality in situations where connectivity is limited or unavailable.

---

## Project Structure

A simplified project structure:

```text
daanph/
|
├── lib/
│   ├── main.dart
│   ├── services/
│   ├── models/
│   ├── screens/
│   └── ...
|
├── assets/
│   ├── db/
│   │   └── commuter.db
│   └── ...
|
├── tools/
│   └── build_offline_db.py
|
├── android/
├── ios/
├── pubspec.yaml
└── README.md
```

---

## Getting Started

### Requirements

* Flutter SDK
* Dart SDK
* Android Studio or another Flutter-compatible development environment
* Git

### Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/daanph.git
cd daanph
```

### Install Dependencies

```bash
flutter pub get
```

### Run the Application

```bash
flutter run
```

Make sure the required offline assets and database are available before running the application.

---

## Testing

DaanPH can be tested using different combinations of Philippine locations and transportation scenarios.

Examples:

```text
Monumento -> Intramuros
Malabon -> Caloocan
Quezon City -> Makati
Manila -> Pasay
Caloocan -> Quezon City
```

Testing should cover:

* Route accuracy
* Transfer instructions
* Fare estimates
* Place search
* Transportation stop search
* Map rendering
* Offline functionality
* Application performance
* Provincial transportation coverage

---

## Development Goals

Future development focuses on:

* Expanding transportation coverage across the Philippines
* Improving route-search accuracy
* Improving fare estimation
* Expanding offline map coverage
* Supporting additional transportation modes
* Improving place and landmark search
* Improving routing performance
* Expanding provincial coverage
* Improving the overall commuter experience

---

## Project Status

**Active Development**

DaanPH is an actively developed project. Transportation coverage, routing capabilities, datasets, and application features may continue to change as the project evolves.

---

## About the Project

DaanPH is an independent software project built in the Philippines with the goal of making public transportation easier to understand and navigate.

The project combines mobile development, geographic data, transportation data, offline databases, and route-search algorithms into a single commuter-focused application.

---

## License

See the repository license for information regarding the use, modification, and distribution of this project.

---

# DaanPH

**Offline public transportation navigation for the Philippines.**
