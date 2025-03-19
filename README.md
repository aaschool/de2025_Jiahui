# de2025_Jiahui_AA Booking System
## Project Overview
The AA Booking System is a smart seat booking system designed for students at the AA Library, ensuring efficient seat reservations and real-time availability tracking. With the help of the system's automated seat management, real-time seat changes, and seamless user interface, students can concentrate on their work without wasting time finding a study spot.

Students book a seat via a React Native mobile app, selecting a time slot first, then a seat. Upon arrival, they check in using an RFID reader, which logs their entry into the system. If they don’t check in within 15 minutes, the CRON system automatically releases the seat. The backend is built with Node.js , providing a REST API for managing bookings, users, and seat status. WebSocket integration ensures real-time seat availability updates, preventing double bookings.

## Project Structure

### Frontend
**React Native** - Handles user interface and interactions

### Backend
**Node.js - API Server** - Manages data, seat reservations, and real-time updates

## Components

### Hardware
* **Mobile Phone** – For seats booking

* **RFID Reader** – For student card check-in at the library entrance

* **AA Card** – For enter library and check in

* **WIFI Rooter** – For check-in devices to the backend server

* **Raspberry Pi** – For connects to RFID reader for processing check-in data


### Software
* **React Native** – For User Interface design

* **WebSocket** – Real-time seat updates

* **Node.js** - Handles API requests and responses.

* **Rest API** - handle user authentication, manage seat reservations, and facilitate communication between the frontend and backend.

* **Cron** - Cancel the reservation If no check-in after 15 minutes by RFID Reader

  
## System Workflow
* **User Login**: The student logs into the app using their AA account credentials, and the backend verifies them.
  
* **Time Slot** Selection: The student selects a preferred study time slot in the app.
  
* **Seat Selection**: The student chooses an available seat from the seat map, and the backend books it.
  
* **Booking Confirmation**: The student confirms the booking, and the backend records the seat reservation with a timestamp.
  
* **RFID Check-in**: The student checks in by scanning their RFID card, and the Raspberry Pi sends the check-in data to the backend.
  
* **Auto-Cancellation**: If no check-in happens within 15 minutes, the backend automatically releases the booked seat.
  
* **View/Manage Bookings**: The student can view or modify their bookings from the app.


## Libraries and References
- https://github.com/wix/react-native-calendars
- https://github.com/18harsh/Movie-Reservation-System
- https://github.com/hemantjayas03/seatBookingApp
- https://github.com/MentorUsama/ReactNativeTicketBooking
- https://github.com/julioalcantara/booking-system
- https://github.com/SunSet1219/Company-workspace-React-Native-
- https://github.com/chandanlog/EVENT-BOOKING-SYSTEM
