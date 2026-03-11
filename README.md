# LaxCoach AI

LaxCoach AI is an applied computer vision system that analyzes lacrosse shooting mechanics using pose estimation and biomechanical metrics.

## Overview

The system allows athletes to record a lacrosse shot on mobile, upload the video for analysis, and receive structured feedback based on pose-derived movement data.

## Problem

Athletes often rely on subjective coaching feedback when evaluating shooting mechanics. LaxCoach AI aims to provide objective, measurable feedback using computer vision.

## Solution

LaxCoach AI uses pose estimation to extract body landmarks from video frames and compute biomechanical metrics such as:

- Hip rotation speed
- Torso velocity
- Arm extension
- Wrist snap

These metrics are translated into actionable feedback for the athlete.

## System Architecture

Mobile App (Flutter)  
↓  
Backend API (FastAPI)  
↓  
Pose Estimation (MediaPipe)  
↓  
Biomechanics Analysis  
↓  
Performance Feedback + Snapshots

## Repositories

- **Backend API:** https://github.com/htgraves/laxcoach-ai-backend
- **Mobile App:** https://github.com/htgraves/laxcoach-ai-mobile

## Tech Stack

- Flutter / Dart
- Python
- FastAPI
- MediaPipe
- OpenCV
- PostgreSQL
- AWS S3

## Example Outputs

- Form score
- Hip speed
- Torso velocity
- Arm extension assessment
- Wrist snap assessment

## My Contribution

I designed and built key parts of the system including:
- backend API development
- pose-based biomechanics metric logic
- video processing workflow
- cloud storage integration
- end-to-end system debugging and iteration
