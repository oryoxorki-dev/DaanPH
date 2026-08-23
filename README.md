# DaanPH

### Offline Public Transportation and Commuter Navigation for the Philippines

**DaanPH** is an offline-first commuter navigation application designed to help Filipinos discover and navigate public transportation routes across the Philippines, even without an internet connection.

The application stores essential transportation, geographic, and map data locally on the device, allowing core search and routing functionality to operate offline.

> DaanPH — Find your way, even offline.

---

## Overview

Navigating public transportation in the Philippines can be challenging, particularly when traveling through unfamiliar areas or when internet connectivity is limited.

DaanPH brings route search, transportation stops, place search, offline maps, and fare estimation together into a single commuter-focused application.

The project is designed specifically around the structure and practical challenges of Philippine public transportation.

---

## Features

### Offline Maps

Locally stored map data allows users to access essential map information without continuously depending on an internet connection.

### Public Transportation Routing

DaanPH searches available transportation data to determine possible routes between an origin and destination.

The routing system can account for multiple transportation services and transfers when determining possible journeys.

### Fare Estimation

DaanPH provides estimated fares for supported transportation routes based on available Philippine public transportation fare data.

Fare information should be treated as an estimate and may change as transportation fares and policies are updated.

### Offline Place Search

Users can search for destinations, landmarks, transportation stops, and other locations using locally stored geographic data.

### Origin and Destination Search

Users can select an origin and destination and receive possible commuting routes between them.

### Offline-First Architecture

Core functionality is designed to operate locally rather than requiring every operation to depend on a remote backend.

Essential transportation and geographic data can be bundled directly with the application.

---

## How It Works

A typical route search follows this process:

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

Route discovery is performed using locally available transportation and geographic data, allowing core routing functionality to remain available without an active internet connection.

---

## Technology

DaanPH is built using the following technologies:

### Mobile Application

* Flutter
* Dart
* Flutter Map
* latlong2

### Local Data and Search

* SQLite
* sqflite
* FTS5 Full-Text Search

### Geographic and Transportation Data

* OpenStreetMap data
* Offline map tiles
* Philippine transportation datasets
* Geographic and place data

The application uses a locally bundled SQLite database to store essential transportation and geographic information required for offline functionality.

---

## Offline Data

DaanPH uses processed transportation and geographic datasets to provide offline commuter functionality.

Depending on the datasets currently included in the application, the data can contain information relating to:

* Jeepneys
* Buses
* Rail transportation
* Public transportation stops
* Transit routes
* Roads
* Places
* Landmarks
* Transportation terminals

Transportation coverage is continuously being expanded and improved as additional datasets become available.

---

## Why Offline?

Many navigation applications depend heavily on:

* Internet connectivity
* Remote APIs
* Online map services
* Cloud-based routing
* Real-time backend services

DaanPH takes an offline-first approach for its core functionality.

By keeping important transportation and geographic data locally available, the application can continue providing essential commuter functionality in situations where connectivity is limited or unavailable.

This approach also reduces the application's dependence on remote services for everyday route searches.

---

## Built for the Philippines

DaanPH is built specifically with Philippine commuters in mind.

The project focuses on making public transportation information easier to search, understand, and navigate.

The long-term goal is to expand transportation coverage, improve route accuracy, and support more areas across the Philippines.

---

## Testing

DaanPH is tested using different Philippine locations and transportation scenarios.

Example journeys include:

```text
Monumento → Intramuros
Malabon → Caloocan
Quezon City → Makati
Manila → Pasay
Caloocan → Quezon City
```

Testing focuses on:

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

## Project Status

**Active Development**

DaanPH is actively developed and tested. Transportation coverage, routing capabilities, datasets, and application features may continue to change as the project evolves.

---

## About DaanPH

DaanPH is an independent software project built in the Philippines with the goal of making public transportation easier to understand and navigate.

The application combines:

* Mobile application development
* Geographic data
* Public transportation data
* Offline databases
* Full-text search
* Route-search algorithms
* Fare estimation
* Offline map technology

into a single commuter-focused application.

---

## Download

The latest Android APK is available through **GitHub Releases**.

For the latest version, visit the repository's **Releases** section.

---

## Developer

**Angeles Micky**

Independent developer and creator of DaanPH, focused on building practical software solutions for Philippine commuters through offline-first mobile technology.

---

## License

See the repository license for information regarding the use, modification, and distribution of this project.
