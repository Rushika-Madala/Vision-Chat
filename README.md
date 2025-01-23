# Vision Chat

## Project Overview
Vision Chat is a real-time communication application with client-server architecture, enabling seamless messaging and potentially vision-related interactions.

On Screen keyboard operated using Eye tracking to identify key presses and releases.
Provides ability to use chat application for mobility impaired individuals.

## Project Structure
```
Vision Chat/
│
├── Client.py         # Client-side application logic
├── Server.py         # Server-side application logic
├── message.py        # Message handling and processing
├── utils.py          # Utility functions and helpers
├── requirements.txt  # Project dependencies
│
└── FILES/            # Trained ML Model Files
    ├── blinkdetection.h5     # Blink detection model
    ├── gazedetection.h5      # Gaze detection model
    ├── gazev4.h5             # Advanced gaze tracking model
    └── shape_predictor_68_face_landmarks.dat  # Facial landmark detection model
```

## Key Components
- `Client.py`: Handles client-side connections and interactions
- `Server.py`: Manages server-side socket connections and message routing
- `message.py`: Implements message processing using image classification and communication protocols for sending message contents
- `utils.py`: Provides utility functions for the application

## Prerequisites
- Python 3.7+
- Required dependencies (list in `requirements.txt`)

## Setup and Running
1. Ensure Python is installed
2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Start the server
```bash
python Server.py
```

4. Start the client
```bash
python Client.py
```

## Features
- Eye tracking
- Real-time messaging
- Client-server communication
- Supports vision-related interactions

## Troubleshooting
- Check firewall settings
- Verify Python and dependency versions



---