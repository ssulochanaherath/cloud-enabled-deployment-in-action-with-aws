## Sangeeth Sulochana
### ID: 2301671096

# Cloud-Enabled Deployment with AWS

This repository demonstrates a cloud-enabled application setup with multiple backend services and a React frontend. All projects are designed to be deployed on AWS.

## Project Overview

- **course-service** → Spring Boot with MySQL
- **student-service** → Spring Boot with MongoDB
- **media-service** → Spring Boot file service (uses local storage by default but can be extended to S3 or MinIO)
- **frontend-app** → React application built with TypeScript, Material UI, Axios, and Vite

---

## Backend Services

### 1. Course Service
- Entity: Course (id, name, duration)
- Endpoints:
  - Get all courses
  - Get a course by ID
  - Add a new course
  - Delete a course
- Runs on port 8081
- Requires MySQL configuration

---

### 2. Student Service
- Document: Student (registration number, full name, address, contact, email)
- Endpoints:
  - Get all students
  - Get a student by ID
  - Add a new student
  - Delete a student
- Runs on port 8082
- Requires MongoDB configuration

---

### 3. Media Service
- Handles file storage and management
- Endpoints:
  - Upload a file
  - List all uploaded files
  - Download a file
  - Delete a file
- Runs on port 8083
- Stores files at `./data/media` by default (can be changed with the `MEDIA_STORAGE_DIR` environment variable)

---

## Frontend Application

The frontend is developed with React and TypeScript, styled using Material UI, and communicates with backend services using Axios. Vite is used as the build tool.

It provides three main sections:
- Courses
- Students
- Media

Available scripts:
- Run the development server
- Build for production
- Preview the production build

---

## Build Instructions

- To build the backend services, run a Maven build at the project root with tests skipped.
- To start the frontend, first install dependencies using npm, then run the development server.
- To prepare the frontend for production, run the build command, and to preview the production build, run the preview script.

---

## Demo

🎥 [Watch the sample screen recording](https://drive.google.com/file/d/1wI0RxUEJIfPWP8RpiC68FmDPuamIcM1h/view?usp=sharing)

---
