# 🛒 E-Commerce Mobile Application

**E-Commerce Application** is a comprehensive, full-featured mobile shopping platform built with Flutter. It provides a complete end-to-end retail experience, featuring distinct interfaces for both buyers and sellers (admins). The application leverages Firebase for robust real-time data management and secure authentication, while integrating Stripe to handle seamless checkout and payment processing.

## ✨ Key Features

* **Dual User Roles (Buyer & Seller):** Offers dedicated dashboards and flows. Buyers can browse, manage their carts, and track orders, while administrators/sellers have a dedicated portal to manage inventory and monitor sales.
* **Secure Payment Integration:** Integrated with the Stripe payment gateway to process secure transactions natively within the app.
* **Advanced Inventory Management:** Sellers can add, edit, and remove products, view comprehensive product lists, and track order fulfillment statuses directly from the administrative interface.
* **Dynamic Shopping Cart:** Utilizes provider-based state management to handle real-time cart updates, ensuring a smooth and responsive checkout experience.
* **Serverless Backend:** Employs Firebase Cloud Functions to securely execute backend logic (like payment intents) without maintaining a dedicated server.

## 🏗️ System Architecture

* **Frontend:** A cross-platform mobile application written in Dart using the Flutter framework.
* **State Management:** Adopts the `Provider` pattern for predictable and scalable application state (e.g., `cart_provider.dart`, `product_stats_provider.dart`).
* **Backend as a Service (BaaS):** Relies heavily on Firebase for core infrastructural needs, including Authentication (`login_page.dart`, `signup_page.dart`) and Firestore for NoSQL data persistence.

## 🛠️ Tech Stack

* **Framework:** Flutter & Dart
* **Backend Services:** Firebase (Auth, Cloud Firestore, Cloud Functions)
* **Payment Gateway:** Stripe
* **State Management:** Provider

## 🚀 Getting Started

### Prerequisites
* Flutter SDK (Latest stable)
* Dart SDK
* Firebase CLI (for deploying functions)
* Stripe Developer Account (for API keys)

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/yourusername/e-commerce-application.git](https://github.com/yourusername/e-commerce-application.git)
    cd e-commerce-application
    ```

2.  **Install Flutter dependencies:**
    ```bash
    flutter pub get
    ```

3.  **Environment Setup:**
    * Configure Firebase for your local project (`lib/firebase_options.dart` generation via FlutterFire CLI).
    * Update your Stripe Publishable Key and Secret Key in the application's configuration/constants file.

4.  **Deploy Cloud Functions (Optional but required for payments):**
    ```bash
    cd functions
    npm install
    firebase deploy --only functions
    ```

5.  **Run the application:**
    ```bash
    flutter run
    ```

---
## 👨‍💻 About the Developer
Engineered by **Ajijolaoluwa Adesoji**, Full-Stack & AI Engineer. This repository highlights the ability to architect complex, production-ready mobile applications featuring multiple user flows, cloud-based data synchronization, and integrated financial services.
