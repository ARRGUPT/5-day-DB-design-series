# 🛗 Day 5: Smart Elevator Control System Database Design

## 🧠 Problem

A growing infrastructure technology company needs a smart elevator control platform to manage elevators across multiple commercial buildings, malls, airports, hospitals, and residential complexes.

The goal is to design a database that can handle:

* Multiple buildings and floors
* Multiple elevators operating within a building
* Elevator-to-floor servicing relationships
* Floor request tracking
* Ride assignment and ride history
* Elevator status monitoring
* Maintenance management

## 🔥 Key Challenges

* One building contains multiple floors and elevators
* Multiple elevators can serve the same floor
* One elevator can serve multiple floors
* Floor requests must be assigned to elevators efficiently
* Ride activity should be separated from elevator configuration
* Maintenance history should be tracked without affecting operational data

## 💡 Solution

* Created separate entities for buildings, floors, elevators, and elevator shafts
* Used an `elevator_floor` junction table to model the many-to-many relationship between elevators and floors
* Separated floor requests from ride assignments and ride logs
* Added maintenance tracking to maintain service history
* Stored elevator status independently for operational monitoring

## 🧱 Entities

* Buildings
* Floors
* Elevators
* Elevator Shafts
* Floor Requests
* Ride Assignments
* Ride Logs
* Elevator-Floor Mapping
* Maintenance

## 📊 ER Diagram

![ER Diagram](/day-05-smart-elevator-control-system/Screenshot%202026-05-30%20214728.png)

## 🚀 Learning

This helped me understand:

* Designing infrastructure management systems
* Modeling many-to-many relationships using junction tables
* Separating static configuration data from dynamic operational data
* Tracking requests, assignments, and ride history independently
* Managing maintenance records without affecting system operations

---

Day 5 complete ✅