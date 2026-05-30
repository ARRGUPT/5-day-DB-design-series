# 🏥 Day 3: Clinic Appointment & Diagnostics Platform Database Design

## 🧠 Problem

A modern clinic wants to digitize its operations and manage appointments, consultations, diagnostic tests, reports, and payments efficiently.

The goal is to design a clean database that can handle:

* Multiple doctors across different specialties
* Patient appointment scheduling
* Consultation and visit tracking
* Diagnostic test prescriptions
* Report generation and delivery
* Payment management

## 🔥 Key Challenges

* One patient can book multiple appointments
* An appointment may or may not result in a consultation
* One doctor can attend many patients
* A consultation can prescribe multiple diagnostic tests
* Reports are generated later and must be linked to the correct test
* Payments should be connected to actual clinic visits and services

## 💡 Solution

* Used `appointments` to manage booking and appointment status
* Created a separate `consultations` table to distinguish scheduled appointments from actual visits
* Linked diagnostic tests to consultations since tests are prescribed during visits
* Connected reports directly to diagnostic tests for accurate report tracking
* Maintained a separate payments table to support flexible billing and payment records

## 🧱 Entities

* Doctors
* Patients
* Appointments
* Consultations
* Diagnostic Tests
* Reports
* Payments

## 📊 ER Diagram

![ER Diagram](/day-03-clinic-appointment-and-diagnostics-platform/Screenshot%202026-05-30%20153416.png)

## 🚀 Learning

This helped me understand:

* Difference between appointments and actual consultations
* Designing healthcare workflows using relational databases
* Modeling one-to-many relationships effectively
* Structuring diagnostic and reporting systems
* Connecting business processes through proper foreign key relationships

---

Day 3 complete ✅