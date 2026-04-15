# Al Mansour Admin Dashboard 🚀

**A Premium Flutter Web Dashboard for Educational and Stationery Management.**

This dashboard is built for the **Al Mansour** platform, providing a high-performance, professional interface for managing educational content (courses, lessons, teachers) and stationery products with complex variants and stock management.

---

## 🌟 Demo Overview

The dashboard serves as a central hub for administrators to:

- **Monitor** platform activity with real-time statistics.
- **Manage** a wide range of stationery products, from simple items to complex products with multiple variants (color, size, etc.).
- **Organize** the educational curriculum, including teacher profiles, courses, subjects, and student data.
- **Configure** platform-wide settings like sliders, categories, and authentication rules.

---

## 🛠️ Technical Excellence

This project is a showcase of advanced Flutter development practices, focusing on **performance**, **maintainability**, and **clean code**.

### 🏗️ Architecture & Design Patterns

- **Clean Architecture**: Strictly organized into **Data**, **Domain**, and **Presentation** layers. This ensures clear boundaries and makes the codebase highly testable and scalable.
- **Dependency Injection**: Use of `get_it` and code generation with `injectable` to manage service lifetimes and promote loose coupling.
- **State Management (Cubit/BLoC)**: Robust and predictable state management using `flutter_bloc`. Each feature is powered by focused Cubits that handle business logic independently.
- **Advanced Navigation**: Implementation of `go_router` with **URL Path Parameters** (`:id`). This is crucial for Flutter Web to support browser refresh while retaining state and enabling deep linking.

### ⚡ Optimization Techniques

- **ValueKey & BlocSelector**: Precise widget rebuilding by targeting specific state slices and using unique keys to maintain widget identity during list operations.
- **Modular Widgets**: Refactored monolithic screens into self-managed, stateful sub-components (e.g., Image Gallery, Options Section, Variants Table) for maximum readability and reduced memory footprint.
- **Shimmer Effects**: Professional loading skeletons implemented for a high-end user experience during data fetching.

### 🎨 UI/UX Features

- **Custom Animations**: Smooth transitions using `AnimatedSwitcher`, `Hero` (where applicable), and custom curves for a premium "native-like" feel.
- **Lottie & Micro-animations**: Integrated Lottie animations for interactive feedback.
- **Adaptive & Responsive**: Layouts designed to work seamlessly across different screen sizes.
- **Comprehensive UX**: Integrated `toastification` for feedback, `gap` for consistent spacing, and `dotted_border` for interactive areas.

---

## 📸 Feature Gallery

Below you will find visual demonstrations of the core features.

### 🏠 Main Dashboard & Platform Setup

| Feature                   | View 1                                                     | View 2                                                     |
| :------------------------ | :--------------------------------------------------------- | :--------------------------------------------------------- |
| **Sliders Management**    | <img src="assets/screen_shots/slider1.png" width="400"/>   | <img src="assets/screen_shots/slider2.png" width="400"/>   |
| **Categories Management** | <img src="assets/screen_shots/category1.png" width="400"/> | <img src="assets/screen_shots/category2.png" width="400"/> |

---

### 🛍️ Product & Stationery Management

| Feature                       | View 1                                                    | View 2                                                    |
| :---------------------------- | :-------------------------------------------------------- | :-------------------------------------------------------- |
| **Product List & Table**      | <img src="assets/screen_shots/product1.png" width="400"/> | <img src="assets/screen_shots/product2.png" width="400"/> |
| **Complex Variant Generator** | <img src="assets/screen_shots/product3.png" width="400"/> | <img src="assets/screen_shots/product4.png" width="400"/> |

---

### 📚 Educational Content

| Feature                 | View 1                                                    | View 2                                                    |
| :---------------------- | :-------------------------------------------------------- | :-------------------------------------------------------- |
| **Courses**             | <img src="assets/screen_shots/courses1.png" width="400"/> | <img src="assets/screen_shots/courses2.png" width="400"/> |
| **Classes**             | <img src="assets/screen_shots/classes1.png" width="400"/> | <img src="assets/screen_shots/classes2.png" width="400"/> |
| **Teacher Management**  | <img src="assets/screen_shots/teacher1.png" width="400"/> | <img src="assets/screen_shots/teacher2.png" width="400"/> |
| **Notes & Materials**   | <img src="assets/screen_shots/notes1.png" width="400"/>   | <img src="assets/screen_shots/notes2.png" width="400"/>   |
| **Subjects & Students** | <img src="assets/screen_shots/subjects.png" width="400"/> | <img src="assets/screen_shots/students.png" width="400"/> |

---

## 🧰 Technology Stack

### Core

- **Framework**: Flutter (Web/Desktop)
- **Language**: Dart
- **Base Style**: Vanilla CSS-inspired Material Design with Custom Components

### State & Navigation

- **State Management**: `flutter_bloc` (Cubit)
- **Routing**: `go_router` (Nested Routes & Path Parameters)
- **DI**: `get_it` & `injectable`

### Data & Networking

- **API Client**: `Dio` (with interceptors and logging)
- **Functional Programming**: `dartz` (Either for Error Handling)
- **Persistence**: `shared_preferences`

### UI Enhancements

- **Images**: `cached_network_image`, `flutter_svg`, `image_picker`
- **Feedback**: `toastification`, `shimmer`, `gap`, `dotted_border`
- **Animations**: `lottie`, `flutter_animate`

---

## 🚀 Getting Started

1. **Clone the repository:**

   ```bash
   git clone https://github.com/AhmedNasser24/almansour_admin.git
   ```

2. **Install dependencies:**

   ```bash
   flutter pub get
   ```

3. **Generate code (Injectable):**

   ```bash
   flutter pub run build_runner build --delete-conflicting-outputs
   ```

4. **Run the project:**
   ```bash
   flutter run -d chrome
   ```
