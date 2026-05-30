# 🚗 Day 4: Comic-Con Parking System Database Design

## 🧠 Problem

A large convention venue hosting Comic-Con India needs a parking management system to handle thousands of vehicles arriving across multiple event days.

The goal is to design a database that can manage:

* Different vehicle types
* Multi-zone parking facilities
* Parking spot allocation
* Reserved parking categories
* Entry and exit tracking
* Ticket generation
* Parking fee calculation
* Payment management

## 🔥 Key Challenges

* One vehicle can visit the venue multiple times during the event
* One parking spot can be reused across many parking sessions
* Different vehicle types require suitable parking spots
* Reserved spots must support VIP guests, exhibitors, staff, and EV charging vehicles
* The system must track currently parked vehicles
* Payments should be linked to parking sessions

## 💡 Solution

* Created a dedicated `parking_sessions` table to track vehicle entry, exit, parking duration, and fees
* Used separate entities for vehicles, parking zones, parking spots, tickets, and payments
* Linked parking spots to parking zones for multi-zone parking management
* Stored parking spot categories directly within parking spots for reserved parking allocation
* Connected tickets and payments directly to parking sessions for accurate tracking

## 🧱 Entities

* Vehicles
* Parking Zones
* Parking Spots
* Parking Sessions
* Parking Tickets
* Payments

## 📊 ER Diagram

![ER Diagram](/day-04-comic-con-parking-system/Screenshot%202026-05-30%20180641.png)

## 🚀 Learning

This helped me understand:

* Designing a real-world parking management system
* Modeling reusable parking spots across multiple sessions
* Tracking vehicle entry and exit using session-based design
* Managing parking allocation across zones
* Structuring ticketing and payment workflows with proper relationships

---

Day 4 complete ✅