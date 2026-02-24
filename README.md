# AI-Based Attendance Tracking System
# Project Overview

This project is an AI-based attendance tracking system that automatically records employee attendance using facial recognition technology. The system is trained on images of registered employees and uses a live camera feed to detect and identify individuals in real time.

When a registered employee is recognized for the first time on a given day, their name, date, and time are recorded in a CSV or Excel file. The system ensures that duplicate entries for the same person on the same day are not created. If an unknown individual appears, the system ignores them without recording any data.

# Features

Real-time face detection and recognition using a live camera feed

Automatic attendance logging with name, date, and time

Prevention of duplicate entries for the same day

Ignores unregistered or unknown individuals

Stores attendance records in CSV or Excel format

# Technologies Used :

Python

OpenCV

Face Recognition library

NumPy

Pandas

# How It Works

The system loads and encodes images of registered employees.

A live video feed is captured using a webcam.

Faces in each frame are detected and compared with stored encodings.

If a match is found:

The employee’s name, current date, and time are recorded.

The system checks if attendance for that person has already been marked for the day to prevent duplicates.

If no match is found, the system ignores the individual.

# Output

The attendance file contains:

Employee Name

Date

Time

Each employee is marked only once per day.
