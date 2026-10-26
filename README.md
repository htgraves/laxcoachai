# LaxCoach AI

LaxCoach AI is an AI-powered lacrosse coaching application that uses computer vision and biomechanical analysis to help athletes evaluate their shooting mechanics and track performance over time.

The application is publicly available on iOS and combines mobile development, backend APIs, computer vision, video processing, and cloud infrastructure.

## Overview

LaxCoach AI allows athletes to record or upload lacrosse shooting videos and receive structured performance feedback based on pose-derived movement metrics.

The platform also includes player performance history and coaching functionality that enables coaches to review athletes' shots, provide feedback, and manage teams.

## Problem

Evaluating lacrosse shooting mechanics traditionally relies on visual observation and subjective coaching feedback.

Athletes may struggle to identify specific mechanical issues, measure improvements, or consistently track their development.

LaxCoach AI aims to make technical feedback more accessible by using computer vision to extract measurable movement data from shooting videos.

## Solution

LaxCoach AI processes uploaded shooting videos using pose estimation and custom biomechanics analysis.

The system evaluates metrics such as:

- Hip rotation speed
- Torso velocity
- Shooting arm extension
- Torso rotation and coil
- Forward weight transfer
- Shooting elbow positioning
- Wrist movement

These measurements support structured feedback that helps athletes better understand their shooting mechanics.

The application also provides:

- Video-based shooting analysis
- Performance history and progress tracking
- Analysis snapshots and video playback
- User authentication and subscription management
- Team management and coach-player functionality
- Coach feedback and drill assignments

## System Architecture

Flutter Mobile Application  
↓  
FastAPI Backend  
↓  
Video Upload & Validation  
↓  
FFmpeg Video Normalization  
↓  
MediaPipe Pose Estimation  
↓  
Custom Biomechanics Analysis  
↓  
Performance Metrics & Feedback  
↓  
PostgreSQL + AWS S3  
↓  
Player History & Coaching Interface

## Tech Stack

### Mobile Application
- Flutter
- Dart

### Backend
- Python
- FastAPI
- PostgreSQL
- SQLAlchemy
- Alembic

### Computer Vision & Video Processing
- MediaPipe
- OpenCV
- FFmpeg
- Custom biomechanics analysis

### Infrastructure & Services
- AWS S3
- Render
- RevenueCat
- Twilio
- Sentry

## Engineering Highlights

### Full-Stack Application Development

Designed and developed an iOS application supported by a Python/FastAPI backend, relational database, and cloud-based media storage.

Implemented API endpoints, database models, authentication, and application workflows supporting both athletes and coaches.

### Computer Vision & Biomechanics Analysis

Integrated MediaPipe pose estimation to extract body landmarks from shooting videos.

Developed custom analysis logic to calculate movement metrics, including torso rotation, arm extension, weight transfer, and elbow positioning.

### Video Processing Pipeline

Built a video-processing workflow that validates uploaded files, normalizes video formats using FFmpeg when needed, performs pose-based analysis, and stores results and media in AWS S3.

Implemented background video conversion to improve playback compatibility after the primary analysis completes.

### Authentication & Data Security

Implemented JWT-based authentication, role-restricted API endpoints, and user-scoped access controls for player data and video content.

### Database Design & Performance Tracking

Designed PostgreSQL schemas to store player information, shooting analysis results, performance history, and coaching-related data.

Used Alembic migrations to manage database schema changes as the application evolved.

### Production Monitoring & Reliability

Maintain the deployed application using Sentry, backend logging, automated tests, and Render deployments.

Investigate production issues, troubleshoot backend failures, and verify changes before release.

## Coaching Platform

In addition to individual shooting analysis, LaxCoach AI includes functionality for coaches to manage players, review shooting videos, provide feedback, and assign drills.

The coaching platform is currently in beta with Quinnipiac University's men's lacrosse program.

## My Contribution

I founded LaxCoach AI and am responsible for its technical development and ongoing maintenance.

My work includes:

- Application architecture and system design
- Flutter mobile application development
- Python/FastAPI backend development
- Computer vision integration and custom biomechanics logic
- Video processing and cloud storage
- Database design and migrations
- Authentication and authorization
- Coaching features and player management
- Testing, debugging, deployment, and production maintenance

## Project Status

LaxCoach AI is a publicly available iOS application with approximately 400 downloads.

The core shooting analysis application is released, while additional coaching features are being developed and tested.

## Code Availability

LaxCoach AI is a privately developed commercial application under active development.

The full source code is not publicly available.

This repository provides a technical overview of the system, its architecture, and the engineering work involved.
