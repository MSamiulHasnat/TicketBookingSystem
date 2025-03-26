# TicketBookingSystem
A Flight Booking System built as part of a DBMS course, focusing on SQL operations such as table creation, relationships, transactions, and queries. The system allows passengers to book flights, make payments, and manage bookings. Includes database schema, sample data, and SQL queries for full functionality.

# Flight Booking System - DBMS Project

## Project Overview
This project is a Flight Booking System that allows passengers to book flights, make payments, and manage their bookings. It is designed as part of the Database Management Systems (DBMS) course and focuses on applying SQL concepts like table creation, relationships, transactions, and queries to build a fully functional system.

The system includes the following main components:
- **Passengers**: User data for flight bookings.
- **Flights**: Information about available flights.
- **Tickets**: Booking information, including seat numbers and statuses.
- **Payments**: Details about the payment transactions for booked tickets.

## Features
- **Passenger Booking**: Search for available flights and book tickets.
- **Payment Processing**: Make payments for booked tickets.
- **Flight Search**: Search flights by departure/arrival airports, date, and availability.
- **Ticket Cancellation**: Cancel tickets and manage booking status.
- **Reporting**: Generate reports on booking status, available seats, and total revenue.
- **Admin Panel**: Manage flight schedules, booking statuses, and payments.

## Database Design
The project uses a relational database with the following core entities:

- **Passengers**
  - Stores passenger details like name, contact info, passport number, etc.
- **Flights**
  - Stores flight details such as flight number, departure/arrival airports, and seat availability.
- **Tickets**
  - Stores ticket booking details, linked to both passengers and flights.
- **Payments**
  - Stores payment transaction details associated with booked tickets.

### Relationships:
- **Passenger ↔ Ticket**: One passenger can book multiple tickets.
- **Ticket ↔ Flight**: Each ticket is associated with one flight, and a flight can have multiple tickets.
- **Ticket ↔ Payment**: A ticket can have multiple payments (in case of split payments).

## SQL Operations Implemented
- **Create Tables**: Used `CREATE TABLE` to define tables for passengers, flights, tickets, and payments.
- **Insert Data**: Inserted sample data using `INSERT INTO`.
- **Queries**: Performed joins to fetch data for passengers, tickets, flights, and payments.
- **Transactions**: Implemented transactions to ensure data integrity when booking a flight and processing payments.
- **Normalization**: Ensured database normalization to 3NF to avoid data redundancy.

## Installation Instructions

### Prerequisites
- SQL Database (e.g., MySQL, PostgreSQL, etc.)
- A SQL client (e.g., MySQL Workbench, DBeaver)

### Steps
1. Clone this repository:
   ```bash
   git clone https://github.com/MSamiulHasnat/TicketBookingSystem.git

/flight-booking-system
│
├── /data/
│   ├── flight_booking_system_schema.sql   # SQL schema file
│   └── sample_data.sql                    # SQL script for inserting sample data
│
├── /queries/
│   ├── booking_query.sql                  # SQL query for booking a ticket
│   ├── payment_query.sql                  # SQL query for processing payment
│   └── cancel_ticket_query.sql            # SQL query for ticket cancellation
│
├── README.md                              # Project documentation
└── LICENSE                                # License for this project
![image](https://github.com/user-attachments/assets/b525a706-adfa-4287-98e5-f14fadd86207)
