# Logistiqo – Transport & Warehouse Management Platform

---

# 🚀 Marketing Overview

## What is Logistiqo?

**Logistiqo is a cloud-based Transport Management System (TMS) and Warehouse Execution System (WES)** built for modern logistics operations.

It connects **transport, warehouse, air cargo, passenger transport, and emergency services** into one unified platform.

👉 Instead of using multiple disconnected systems, Logistiqo provides **one system for the entire logistics chain**.

---

## Why Companies Use Logistiqo

* Reduce manual work through automation
* Improve planning and dispatching efficiency
* Gain real-time visibility across operations
* Replace multiple legacy systems with one platform
* Scale across locations and countries

---

## Key Capabilities

### 🚚 Transport Management (TMS)

* Dispatching of drivers and vehicles
* Route and tour planning
* Real-time tracking and updates
* Automatic scheduling based on rules

### 📦 Warehouse Execution (WES)

* Inbound and outbound handling
* Storage and picking
* Full traceability
* No need for a separate warehouse system

### ✈️ Air Cargo & Airport Operations

* AWB / HAWB handling
* ULD build-up and breakdown
* RFS (Road Feeder Service)
* Security (RA/KC) and customs
* FSU event handling

### 🤖 Automation & AI

* Automatic creation of tours and manifests
* AI-assisted document import (PDF, email, AWB, BOL)
* Reduced manual data entry

---

## Who Uses Logistiqo?

* Freight forwarders
* Transport companies
* Warehouse operators
* Airport cargo handlers
* Passenger transport providers
* Emergency service providers (PERS)

---

## Proven in Production

Logistiqo is already used in real operations, including:

* Frankfurt Airport
* Vienna
* Graz
* Helsinki

---

## One Platform Instead of Many

Logistiqo combines:

* Transport Management System (TMS)
* Warehouse Execution System (WES)
* Air Cargo Handling System
* Passenger & Emergency Transport System

👉 Result: **Full control over your logistics operations in one system**

---

# 🧭 User Guide / How It Works

## Core Concept: Shipment-Centric System

Everything in Logistiqo is based on the **shipment**.

Depending on the shipment type, the system automatically adapts:

* Cargo → Sender / Receiver
* Passenger → Pickup / Destination
* Emergency → Incident / Response

---

## Typical Workflow

### 1. Create or Import Shipment

Shipments can be:

* Entered manually
* Imported via API
* Extracted automatically from documents (AI)

---

### 2. Plan Transport or Handling

Logistiqo can:

* Assign vehicles and drivers
* Plan routes and tours
* Consider constraints such as:

  * Time windows
  * Capacity
  * Volume / weight

---

### 3. Warehouse Processing (if applicable)

* Receive goods (inbound)
* Store and manage inventory
* Pick and prepare shipments
* Handle outbound processes

---

### 4. Execution & Tracking

* Drivers receive tasks (mobile app)
* Status updates in real time
* Events like loading, departure, arrival are recorded

---

### 5. Completion & Documentation

* Proof of delivery / completion
* Status updates finalized
* Data available for invoicing and reporting

---

## Automation Logic

Logistiqo can automatically create:

* Tours
* Manifests
* Transport plans

Based on:

* Slot times
* Vehicle capacity
* Shipment volume
* Pallet constraints

---

## Integration

Logistiqo provides APIs to:

* Exchange data with customers and partners
* Integrate external systems
* Automate workflows

---

## Real-World Examples

### ✈️ Air Cargo Workflow (AWB)

1. AWB is imported (API, EDI, or AI from document)
2. Shipment is created automatically
3. Goods are received in the warehouse
4. ULD build-up is performed
5. Transport to airport or handling agent is planned
6. FSU events are generated and tracked

👉 Result: Full traceability from document to flight

---

### 🚚 Transport Workflow (Road)

1. Shipment is created (manual or API)
2. System assigns vehicle and driver
3. Tour is automatically generated
4. Driver receives tasks on mobile app
5. Pickup → stopovers → delivery executed
6. Status updates in real time

👉 Result: Optimized routing and full visibility

---

### 🚑 Emergency / PERS Workflow

1. Emergency request is received
2. Closest available vehicle is identified
3. Task is dispatched immediately
4. Driver navigates to customer
5. Status and timing are tracked

👉 Result: Fast response with controlled execution

---

## Technical Architecture

### Architecture Overview

Logistiqo is built as a **cloud-based, multi-tenant logistics platform** with a central backend, web frontend, mobile applications, APIs, and automation services.

The architecture is designed around one core principle:

> The shipment is the central business object.

Transport, warehouse, air cargo, passenger transport, emergency transport, manifests, tours, status events, and invoicing are all connected through shipment-related data.

---

### Main Components

#### 1. Web Application

The web application is used by dispatchers, warehouse users, administrators, and operational teams.

It provides:

* Shipment management
* Planning and dispatching
* Timeline / scheduling views
* Warehouse handling screens
* Master data management
* Reporting and invoicing workflows

The platform is moving toward a modern **React-based frontend** for improved performance, usability, and maintainability.

---

#### 2. Backend Services

The backend contains the business logic for shipment handling, transport planning, warehouse execution, status processing, invoicing, and integrations.

Typical backend responsibilities include:

* Shipment lifecycle management
* Tour and manifest creation
* Driver and vehicle assignment
* Status and event processing
* Customer-specific rules
* Permission and domain handling
* API processing

The backend is service-oriented, with logic separated into controllers, services, repositories, and DTOs.

---

#### 3. Database Layer

Logistiqo uses a relational database structure where customer and operational data are stored in structured tables.

Core data areas include:

* Shipments
* Shipment details
* Transport services
* Vehicles and drivers
* Addresses and companies
* Warehouse and ULD data
* Status history
* Invoices and accounting data
* Domain and customer settings

The system supports customer-specific configuration through domain settings and rule-based behavior.

---

#### 4. Mobile Applications

Drivers and operational staff use mobile apps to receive and execute tasks.

Mobile functionality includes:

* Task lists
* Pickup and delivery confirmation
* Barcode scanning
* Photo capture
* Proof of delivery
* Real-time status updates
* Emergency alerts where required

The mobile apps synchronize with the backend and support field operations in real time.

---

#### 5. API Layer

Logistiqo provides APIs for external systems, partners, and customers.

The API layer is used for:

* Creating and updating shipments
* Exchanging status information
* Importing customer orders
* Connecting warehouse and transport partners
* Integrating external planning, accounting, or airport systems

APIs allow Logistiqo to act as an integration platform between logistics participants.

---

#### 6. Automation Engine

Automation is a major part of Logistiqo.

The system can automatically create:

* Tours
* Manifests
* Transport plans
* Warehouse handling tasks
* Status-based follow-up actions

Automation rules may consider:

* Slot times
* Vehicle capacity
* Driver availability
* Shipment volume and weight
* Euro-pallet limits
* Customer-specific planning rules
* Shipment type

---

#### 7. Real-Time Communication

Logistiqo supports real-time operational updates between backend, web frontend, and mobile devices.

This enables:

* Live shipment status updates
* Dispatcher visibility
* Driver communication
* Timeline updates
* Emergency notifications
* Operational alerts

---

#### 8. AI-Assisted Processing

AI is used to reduce manual work and improve data capture.

AI-assisted workflows may include:

* Reading shipment data from emails
* Extracting AWB / BOL information from PDFs
* Suggesting missing shipment data
* Supporting document-based imports
* Assisting users during data entry

AI is used as an assistant to improve efficiency, while operational control remains with the user and system rules.

---

### Architecture Goals

The technical architecture is designed to support:

* Scalability across many customers and locations
* Multi-domain logistics operations
* High configurability per customer
* Real-time execution
* API-driven integrations
* Gradual modernization toward React and service-based architecture
* Reliable operations for mission-critical logistics processes

---

## Summary

Logistiqo is a **shipment-driven logistics platform** that combines planning, execution, and automation across transport and warehouse operations.

It is designed to support both **daily operations (user workflows)** and **strategic growth (scalable architecture)**.
