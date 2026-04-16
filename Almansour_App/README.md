# Al-Mansour Application 📱🎓

Welcome to the **Al-Mansour App** repository! This project is a comprehensive cross-platform mobile application tailored for educational services, course bookings, and integrated e-commerce. Built with scalability and maintainability in mind, it leverages industry-standard architectures and modern Flutter technologies.

---

## 🚀 Project Overview

The Al-Mansour App acts as a centralized hub for students and users bridging e-learning and physical product commerce. The platform allows users to:

- **E-Commerce:** Browse educational products, manage their cart, save favorites, and track order history.
- **E-Learning:** Browse subjects, download notes, and seamlessly book online courses with specific teachers.
- **Engagement:** Participate in real-time Gamification (Wheel of Fortune competitions) and connect via Live Chat.
- **Logistics:** Pinpoint precise delivery locations via interactive Google Maps integrations.

---

## 🛠️ Tech Stack & Skills Demonstrated

This project is a massive testament to writing enterprise-level, production-ready Flutter code.

### 🏛️ Architecture

- **Clean Architecture:** Strict separation of concerns divided horizontally into `Presentation`, `Domain`, and `Data` layers.
- **Feature-First Structure:** Organized strictly by feature (e.g., `/chat`, `/cart`, `/competition`) ensuring high cohesion, modularity, and easy scaling.

### 🧩 State Management & Dependency Injection

- **Bloc / Cubit:** Robust reactive state management handling explicit states natively (Loading, Success, Failure).
- **Injectable / GetIt:** Code-generated Dependency Injection bridging Data Sources to Repositories, UseCases, and Cubits autonomously.

### 🔌 API & Networking

- **Dio:** Configured interceptors for secure Token injections and centralized error handling (`safeApiCall`).
- **WebSockets (Socket.io):** Real-time bidirectional event streaming utilized extensively in the Live Chat feature.

### 🗺️ Native & Third-Party Integrations

- **Google Maps:** Native map clustering and coordinate picking for physical delivery routing.
- **GoRouter:** Advanced declarative deep-link supported routing.
- **Easy Localization:** Seamless multi-language support mapped natively.
- **URL Launcher:** Deep linking for phone, email, and social networks gracefully.

---

## 📱 Feature Demonstrations

_(Note: Replace the placeholder image links with actual screenshots or GIFs when presenting)_

### 1. Home & Main Dashboard

A dynamic, localized entry point highlighting active banners, quick product categories, and immediate access to core flows.
<br>
<img src="Almansour_App/screen_shots/home.png" width="300">

### 2. Comprehensive E-Commerce (Cart, Orders, Products)

Users can filter products natively, manage their local cart, add favorites, and checkout seamlessly.
<br>

<p float="left">
  <img src="Almansour_App/screen_shots/product.png" width="250">
  <img src="Almansour_App/screen_shots/product_details1.png" width="250">
  <img src="Almansour_App/screen_shots/cart.png" width="250">
</p>

### 3. Online Booking & Subject Notes

A dedicated educational space featuring interactive bottom-sheet filters with real-time Cubit State tracking, Shimmer loading loops, and Teacher specific querying.
<br>

<p float="left">
  <img src="Almansour_App/screen_shots/courses.png" width="250">
  <img src="Almansour_App/screen_shots/notes.png" width="250">
  <img src="Almansour_App/screen_shots/classes.png" width="250">
</p>

### 4. Interactive Gamification (Competitions)

A specialized Wheel of Fortune module communicating with the backend to sync live timers and spin physics resolving into exact Winner models safely.
<br>

<p float="left">
  <img src="Almansour_App/screen_shots/wheel1.png" width="250">
  <img src="Almansour_App/screen_shots/wheel2.png" width="250">
</p>

### 5. Real-Time Chat (Socket.io)

Live technical support and user communication streams featuring optimized UI list bubbling mimicking native messenger apps.
<br>
_(Real-time chat supports instant updates mapped to socket protocols)_

### 6. Address & Google Maps Integration

Dynamic spatial polling allowing users to manually pinpoint delivery coordinates bounding against Google Map configurations.
<br>

<p float="left">
  <img src="Almansour_App/screen_shots/address1.png" width="250">
  <img src="Almansour_App/screen_shots/address_with_google_map.png" width="250">
</p>

### 7. Authentication & Profile Management

Full JWT-capable authorization flow covering OTP inputs, password recovery, and secure profile management.
<br>

<p float="left">
  <img src="Almansour_App/screen_shots/login.png" width="250">
  <img src="Almansour_App/screen_shots/otp.png" width="250">
  <img src="Almansour_App/screen_shots/main_profile.png" width="250">
</p>

---

## 💡 Code Quality & Best Practices

- **Predictable Error Handling:** Mapping raw API exceptions into cleanly parsable Failure objects.
- **UI/UX Finesse:** Hand-crafted smooth UI states utilizing extensive `Shimmer` skeleton loaders masking latency beautifully.
- **Scalable Widgets:** Standardized App Colors, extension wrappers (`ScreenExtension`, `TextStyleExtension`), and generic widgets avoiding duplication.
