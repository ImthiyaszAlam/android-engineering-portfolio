# Prune Consumer App

**A Unified Digital Services Platform for Android**

## Overview

Prune Consumer App is a consumer-facing Android application that brings multiple digital services together in a single platform. It offers an integrated experience across telecom services, mobile recharges, utility bill payments, insurance, ONDC-based commerce, and data usage tracking.

Built using Kotlin and Java, the application combines established Android development practices with modern UI technologies, local data persistence, network integrations, mapping SDKs, analytics, and production monitoring tools.

## Key Features

### Telecom & eSIM
- International SIM packs and eSIM plan selection.
- Telecom operator and plan comparison.
- Order summary and plan review workflows.

### Recharge & Bill Payments
- Prepaid and postpaid mobile recharges.
- Recharge coupon support.
- Electricity bill payment services.

### Insurance
- Free and paid travel and health insurance plans.
- Multi-step traveller information flows.
- Insurance plan review and selection.

### ONDC Commerce
- Integration with the Open Network for Digital Commerce (ONDC).
- Buyer and seller discovery.
- Commerce and order management workflows.

### Data Tracking & Customer Support
- Mobile data usage tracking.
- Shopping cart management.
- In-app customer support chatbot.
- Push notifications through Firebase Cloud Messaging (FCM).

## Architecture

The application follows the **Model–View–ViewModel (MVVM)** architectural pattern, using lifecycle-aware components and asynchronous programming to support maintainable Android development.

- **Presentation:** XML layouts, ViewBinding, DataBinding, and Jetpack Compose.
- **ViewModel:** Presentation logic and UI-related state management using LiveData.
- **Data persistence:** Room for local caching and cart-related data.
- **Networking:** Retrofit and Volley for API communication, with Gson for JSON parsing.
- **Asynchronous execution:** Kotlin Coroutines and Android lifecycle-aware components.

## Technology Stack

| Category | Technologies |
|---|---|
| Languages | Kotlin, Java |
| Architecture | MVVM |
| UI | XML, ConstraintLayout, Jetpack Compose, Material 3 |
| View Binding | ViewBinding, DataBinding |
| Lifecycle & State | LiveData, Lifecycle Components |
| Asynchronous Programming | Kotlin Coroutines |
| Local Persistence | Room |
| Networking | Retrofit, Volley |
| JSON Parsing | Gson |
| Maps & Location | Google Maps SDK, Ola Maps SDK |
| Analytics | Firebase Analytics, Facebook Event Tracker |
| Crash Reporting | Firebase Crashlytics |
| Session Analytics | Microsoft Clarity |
| Push Notifications | Firebase Cloud Messaging |
| Build Optimization | R8, Resource Shrinking |

## Production Engineering

The application includes production-oriented Android build configurations and observability integrations.

- **Optimized release builds:** R8 code shrinking and resource shrinking.
- **Android compatibility:** Minimum SDK 24, target SDK 36, and compile SDK 37.
- **Multidex support:** Enabled in the application configuration.
- **Local data management:** Room-based persistence for supported application features.
- **Monitoring and analytics:** Crash reporting, usage analytics, and session insights.
- **Hybrid UI development:** Existing XML-based interfaces alongside incremental Jetpack Compose adoption.
- **Modular package organization:** Separation of responsibilities across application features.

## Platform

- **Platform:** Android
- **Languages:** Kotlin, Java
- **Architecture:** MVVM
- **UI Technologies:** XML Views, Jetpack Compose
- **Distribution:** Google Play Store

---

*Prune Consumer App is a production Android application combining multiple consumer digital services within a unified mobile experience.*
