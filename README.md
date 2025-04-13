# M.S.A.S
My Embedded Systems Project : Motorcycle Safety Adaptive System 

# Motorcycle Adaptive Safety System

## Introduction

This project introduces a motorcycle safety system designed to mitigate accidents by detecting surrounding vehicles and providing timely warnings to the rider.  The system also implements adaptive speed control to prevent collisions with vehicles ahead.

## Problem Statement

Motorcycles offer less protection than cars, leading to higher risks for riders.  Existing safety systems often fall short in addressing motorcycle-specific safety needs.This project aims to bridge this gap by providing an adaptive safety system for motorcycles.

## Features

* **Vehicle Proximity Detection:** Utilizes sensors to detect vehicles in the motorcycle's danger zones. 
* **Adaptive Speed Control:** Adjusts motorcycle speed to prevent forward collisions.
* **Rider Alerts:** Provides visual warnings to the rider via an LCD.
* **Vehicle Alerts:** Notifies surrounding vehicles using pulsing LEDs.
* **Real-time Operation:** System functions with hard real-time constraints (50-300ms).

## Architecture

The system architecture comprises:

* ESP-32 dual-core microcontroller for parallel task handling. 
* Ultrasonic sensor for front vehicle detection. 
* IR sensors for corner vehicle detection.
* LCD for rider alerts.
* LEDs for vehicle alerts.
* DC motor and driver for speed control simulation.

### Component Layout

![component layout](https://github.com/user-attachments/assets/2dc27ea0-ec26-4550-b10b-6fde77a8dde6)

### System Architecture

![architecture](https://github.com/user-attachments/assets/4fd584c2-e0b8-418c-86a5-61508bda7e7f)


## Hardware Design

<img src="https://github.com/user-attachments/assets/428f6aee-a644-4152-beeb-08a4cb403849" width="600" height="400">

Key hardware components include:

* Ultrasonic Sensor (HC-SR04) for front vehicle detection.
* IR Sensors for corner detection. 
* ESP-32 for system control.
* I2C LCD for rider warnings. 
* L298N Motor Driver for speed control.
* 3V-6V DC Motor for prototype demonstration.
* LEDs for vehicle alerts.
* 3.7V Batteries (2x) for power supply.

## Software Design

The software is designed with two main tasks:

* **Task 1:** Detects vehicles in the danger zone and alerts the rider.
* **Task 2:** Controls motorcycle speed based on front vehicle proximity.

The tasks are managed using FreeRTOS on the ESP-32.

## Testing and Results

The system was tested to ensure real-time performance. Key results include:

* Successful parallel execution of tasks on the ESP-32.
* Task completion within the specified time constraints (20ms - 300ms).

| Task Scheduling Configuration |                                                                                               

## Prototype

![Prototype_2](https://github.com/user-attachments/assets/94bab12f-d95d-494a-b1a1-1d898a97da5a)

A small-scale prototype was developed using 3D printing technology with PLA filament. The design was created in SolidWorks to ensure easy integration of electronic components.

## Conclusion

This project demonstrates a promising approach to enhancing motorcycle safety. By integrating real-time processing and adaptive technologies, it addresses critical safety concerns and lays the groundwork for future advancements in motorcycle safety systems.

## Team Members
* Rudra Vala
* Yulia Isaeva
* David Adegoke
* Nicholas Maliavine
