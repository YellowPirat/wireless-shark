# Wireless Shark - CAN Bus Data Logger & Visualizer

A modern web-based application for real-time CAN bus data logging and visualization. 

## Features

### Real-time CAN Bus Monitoring
- Live data capture via WebSocket connection
- Support for multiple CAN interfaces
- DBC file integration for signal interpretation
- Configurable logging parameters

### Dynamic Visualization
- Customizable dashboard with draggable widgets
- Multiple visualization types:
  - Line charts for time-series data
  - Real-time value displays
  - Hex/Binary data views
  - Table views with signal details
- Auto-updating displays with pause functionality
- Layout persistence across sessions

### Configuration Management
- DBC file upload and management
- CAN interface configuration
- YAML-based logger settings
- Assignment management for CAN sockets and DBC files

## Getting Started

### Prerequisites

Wireless Shark builds on three components: 
- Reverse proxy (We use [Caddy](https://caddyserver.com/) in this example)
- [wireless-shark-frontend](https://github.com/YellowPirat/wireless-shark-frontend)
- [wireless-shark-backend](https://github.com/YellowPirat/wireless-shark-backend)

The backend reads the CAN messages from cansockets and broadcasts them over Websockets, afterwards the frontend receives CAN messages and visualizes them. Finally the reverse proxy unifies both components under one domain. 

### Installation

Follow the instructions of both [frontend](https://github.com/YellowPirat/wireless-shark-frontend?tab=readme-ov-file#getting-started) and [backend](https://github.com/YellowPirat/wireless-shark-backend#getting-started) repositories. An example revese proxy configuration can be find in this repository. 

## License

Wireless Shark is distributed under the terms of the GPL-3.0 license.

## Acknowledgments

Created by TI 5 in WiSe 2024/25
- Ahmet Emirhan Göktaş
- Benjamin Klaric
- Jannis Gröger
- Mario Wegman
- Maximilian Hoffmann
- Stasa Lukic


