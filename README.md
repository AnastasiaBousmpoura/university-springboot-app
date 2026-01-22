# FitTrack – Personal Fitness & Trainer Appointment System

## Project Overview
FitTrack is a **Distributed Systems** project developed at **Harokopio University of Athens**. It is a platform designed to streamline workout organization, manage personal trainer appointments, and track fitness progress through a multi-role architecture.

## System Architecture & User Roles
The system implements complex logic for three distinct roles:
* **Guest**: Can browse available trainers by specialization and area, and register for an account.
* **User (Client)**: Manages a fitness profile (goals like weight loss or muscle gain), books appointments, and logs progress (weight, running time).
* **Trainer**: Manages availability slots, accepts/rejects appointments, and maintains personalized training plans for each client.

## Key Distributed Logic & Business Rules
* **Appointment Validation**: Prevents booking in past dates or overlapping slots for the same trainer.
* **Active Limits**: Enforces a maximum number of active appointments per user.
* **External Integrations**: Integrated (or designed for) a **Weather API** to provide weather updates for outdoor training sessions.

## Technical Stack
* **Backend**: Java with **Spring Boot**
* **Data Management**: Spring Data JPA
* **Tools**: Maven, Git
* **Course**: Distributed Systems (3rd Year)
* **Final Grade**: 9/10

## Features & Implementation
* **RESTful Services**: Clean API design for cross-role communication.
* **Relational Mapping**: Complex Many-to-Many and One-to-Many relationships between Users, Trainers, and Appointments.
* **Concurrency Handling**: Basic logic to ensure no double-booking of the same time slot.

## How to Run
1. Clone the repository.
2. Run `./mvnw spring-boot:run`
3. Access the API endpoints at `http://localhost:8081`.
