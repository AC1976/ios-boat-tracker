# iOS Boat Tracker

An iOS application for visualizing GPS tracks of boats using SwiftUI and MapKit. The app displays position data from multiple boats over time, allowing filtering by boat and date range.

## Features

- Display boat positions on an interactive map
- Filter tracks by specific boat
- Date range selection
- SQLite database integration for efficient data storage
- SwiftUI interface with MapKit integration

## Project Structure

```
ios-boat-tracker/
├── BoatTracker/
│   ├── Models/
│   │   └── BoatPosition.swift
│   ├── Managers/
│   │   └── DatabaseManager.swift
│   ├── Views/
│   │   └── MapView.swift
│   └── ViewModels/
│       └── MapViewModel.swift
└── Scripts/
    └── convert_data.py
```

## Setup

1. Clone the repository
2. Convert your GPS data to SQLite using the provided Python script
3. Add the SQLite database to the Xcode project
4. Build and run the project

## Data Conversion

To convert your GPS data from a DataFrame to SQLite, use the provided Python script:

```bash
python Scripts/convert_data.py
```

## Requirements

- iOS 14.0+
- Xcode 12.0+
- Swift 5.3+
- Python 3.6+ (for data conversion)

## License

MIT License