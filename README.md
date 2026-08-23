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

DaanPH searches available transportation data to determine possible routes between an origin and destination.

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

The general routing process works as follows:

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

## Technology

DaanPH is built using:

* Flutter
* Dart
* Flutter Map
* latlong2
* SQLite
* sqflite
* FTS5 Full-Text Search
* OpenStreetMap data
* Offline map tiles
* Philippine transportation datasets

The application uses a locally bundled SQLite database for essential transportation and geographic data.

---

## Offline Data

DaanPH uses processed transportation and geographic datasets to provide offline commuter functionality.

The data can include information relating to:

* Jeepneys
* Buses
* Rail transportation
* Public transportation stops
* Transit routes
* Roads
* Places
* Landmarks
* Transportation terminals

Transportation coverage depends on the datasets currently included in the application and is continuously being expanded and improved.

---

## Why Offline?

Many navigation applications depend heavily on:

* Internet connectivity
* Remote APIs
* Online map services
* Real-time backend services

DaanPH takes an offline-first approach for its core functionality.

By keeping important transportation and geographic data locally available, DaanPH can continue providing essential commuter functionality in situations where connectivity is limited or unavailable.

---

## Built for the Philippines

DaanPH is built specifically with Philippine commuters in mind.

The project focuses on making public transportation information easier to search, understand, and navigate.

The long-term goal is to expand transportation coverage and improve route accuracy across more areas of the Philippines.

---

## Testing

DaanPH is tested using different Philippine locations and transportation scenarios.

Example journeys include:

```text
Monumento -> Intramuros
Malabon -> Caloocan
Quezon City -> Makati
Manila -> Pasay
Caloocan -> Quezon City
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

DaanPH is an actively developed application. Transportation coverage, routing capabilities, datasets, and application features may continue to change as the project evolves.

---

## About DaanPH

DaanPH is an independent software project built in the Philippines with the goal of making public transportation easier to understand and navigate.

The project combines mobile development, geographic data, transportation data, offline databases, and route-search algorithms into a single commuter-focused application.

---

## Download

The latest Android APK is available in the project's **GitHub Releases**.

---

## Developer

**Angeles Micky**

Independent developer and creator of DaanPH, focused on building practical software solutions for Philippine commuters through offline-first mobile technology

---
## License

See the repository license for information regarding the use, modification, and distribution of this project.

---

**DaanPH — Offline public transportation navigation for the Philippines.**
