# FitTrack – Personal Fitness & Trainer Appointment System

A university project developed as part of the **Distributed Systems** course at **Harokopio University of Athens**.

## Project Overview

FitTrack is a web-based fitness and personal trainer management platform designed to simplify workout organization, appointment scheduling, and fitness progress tracking through a multi-role architecture.

## User Roles & Functionality

The application supports three distinct user roles:

- **Guest:** Browse available trainers by specialization and location, and register for an account.
- **User (Client):** Manage a personal fitness profile, set goals such as weight loss or muscle gain, book appointments, and track progress through metrics such as weight and running time.
- **Trainer:** Manage availability slots, accept or reject appointment requests, and maintain client-related information and training plans.

## Core Business Logic

- **Appointment Validation:** Prevents users from booking appointments in the past or creating overlapping appointments with the same trainer.
- **Active Appointment Limits:** Enforces a maximum number of active appointments per user.
- **Availability Management:** Allows trainers to manage their available appointment slots.
- **Role-Based Functionality:** Provides different features and permissions according to each user's role.

## Features & Implementation

- **RESTful Services:** Provides REST endpoints for communication between the application's components.
- **Relational Data Management:** Uses entity relationships, including One-to-Many and Many-to-Many mappings, to represent users, trainers, and appointments.
- **Booking Conflict Prevention:** Implements validation logic to prevent double-booking of trainer time slots.
- **Authentication & Authorization:** Supports role-based access to application functionality.

## Technologies Used

| Category | Technologies |
|---|---|
| Programming Language | Java 21 |
| Backend Framework | Spring Boot |
| Security | Spring Security, JWT |
| Data Access | Spring Data JPA, Hibernate |
| Database | H2 |
| Frontend | Thymeleaf |
| API | REST |
| API Documentation | OpenAPI / Swagger |
| Build Tool | Maven |
| Version Control | Git |

## Running the Application

### Prerequisites
- Java 21
- Maven

### Execution

1. Clone the repository:

   ```bash
   git clone https://github.com/AnastasiaBousmpoura/university-spring-boot-app.git
