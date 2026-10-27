# Prune Delivery Application

**An Integrated Delivery, Field Operations & EV Rental Platform**

## Overview

Prune Delivery Application is an Android application designed to support delivery operations, quick-commerce fulfillment, telecom activations, and electric vehicle (EV) rentals.

The application serves multiple user roles, including **Delivery Partners (Riders), Field Agents, and Team Leads (TLs)**, providing workflows for rider onboarding, KYC verification, order fulfillment, live location tracking, EV rentals, wallet management, incentives, and operational reporting.

Built using Kotlin and Java, the application combines modern Android UI technologies with real-time communication, background processing, mapping integrations, document verification SDKs, and production monitoring tools to support field operations.

## Key Features

### Rider Onboarding & KYC Verification
- Aadhaar KYC verification using the FRSLABS Atlas SDK.
- PAN card and address verification workflows.
- Document capture and photo upload.
- Camera integration using CameraX.
- Image cropping and processing with uCrop.

### Order Fulfillment & Management
- Real-time incoming delivery order alerts.
- Order acceptance and status management.
- Order rescheduling and completion workflows.
- Return-to-Origin (RTO) and return management.
- Custom floating overlays and high-priority order alerts.
- Lock-screen notification and order interaction workflows.

### EV Rental Ecosystem
- Browse and compare available electric vehicles.
- Select rental vendors and pickup locations.
- Manage rental security deposits and payment statuses.
- Confirm vehicle pickup.
- Track rental-related operational workflows.

### Team Lead & Staff Operations
- Role-based access for riders, field agents, and team leads.
- Monitor ongoing, pending, and reported orders.
- Oversee delivery partner activities.
- Access operational dashboards and reporting workflows.

### Wallet, Incentives & Referrals
- View wallet transaction history.
- Access wallet transfer reports.
- Explore offers and referral programs.
- Track incentives based on shift completion and operational criteria.

## Architecture

The application uses a hybrid Kotlin/Java codebase, combining Jetpack Compose with traditional XML-based Android UI components.

Its implementation incorporates lifecycle-aware Android components, REST API communication, background processing, real-time synchronization, and role-specific workflows.

### Architectural Components

- **UI Layer:** Jetpack Compose with Material 3, XML layouts, ViewBinding, and DataBinding.
- **Networking:** Retrofit and Gson Converter for REST API integration.
- **Background Execution:** Android foreground services and WorkManager for supported background tasks.
- **Location & Navigation:** Google Maps API, Ola Maps SDK, and Uber H3 spatial indexing.
- **Camera & Scanning:** CameraX and Google ML Kit barcode/QR scanning.
- **Identity Verification:** FRSLABS Atlas SDK for KYC workflows.
- **Monitoring:** Firebase Crashlytics, Firebase Analytics, and Microsoft Clarity.

## Technology Stack

| Category | Technologies |
|---|---|
| Languages | Kotlin, Java |
| UI Frameworks | Jetpack Compose, Material 3, XML Layouts |
| View Binding | ViewBinding, DataBinding |
| Networking | Retrofit, Gson Converter |
| Maps & Navigation | Google Maps API, Ola Maps SDK |
| Spatial Indexing | Uber H3 |
| Background Processing | Foreground Services, WorkManager |
| Real-Time Communication | Socket-based synchronization |
| KYC Verification | FRSLABS Atlas SDK |
| Camera & Image Processing | CameraX, uCrop |
| Barcode & QR Scanning | Google ML Kit |
| Crash Reporting | Firebase Crashlytics |
| Analytics | Firebase Analytics |
| Session Analytics | Microsoft Clarity |

## Engineering Highlights

### Reliable Background Execution & Live Tracking
Implemented background-processing workflows using Android foreground services and WorkManager to support rider location tracking and operational synchronization, subject to Android lifecycle and background-execution restrictions.

### Real-Time Order Notifications
Integrated custom order-alert workflows involving alarm receivers, floating overlays, and full-screen activities to help riders respond to high-priority delivery requests, with appropriate Android permission and notification handling.

### Mapping & Spatial Operations
Integrated multiple mapping technologies, including Google Maps and Ola Maps, alongside Uber H3 spatial indexing to support location-aware delivery and navigation workflows.

### Third-Party SDK & Hardware Integration
Integrated native Android capabilities and external SDKs for KYC verification, camera-based document capture, image processing, and barcode/QR scanning.

### Multi-Role Operational Workflows
Organized rider and administrative workflows around distinct user roles, supporting operational visibility and role-specific functionality for delivery partners, field agents, and team leads.

## Production & Operational Scope

The application brings together several operational domains within a unified Android platform:

- Delivery fleet and order lifecycle management.
- Telecom SIM delivery and activation workflows.
- Rider identity verification and onboarding.
- EV rental and vehicle pickup operations.
- Rider incentives, wallet history, and referrals.
- Team lead dashboards and operational reporting.
- Location tracking and real-time order synchronization.

## Platform

- **Platform:** Android
- **Languages:** Kotlin, Java
- **UI:** Jetpack Compose, XML Views
- **Networking:** Retrofit
- **Mapping:** Google Maps, Ola Maps
- **Background Processing:** Foreground Services, WorkManager
- **Monitoring:** Firebase Crashlytics, Firebase Analytics, Microsoft Clarity

---

*Prune Delivery Application is a production-oriented Android solution for managing delivery operations, field teams, rider onboarding, location-aware workflows, and EV rental services within a unified platform.*
