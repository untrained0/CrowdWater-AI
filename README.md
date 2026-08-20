# SmartWater System

Welcome to the SmartWater System project repository. This project is a comprehensive, AI-powered solution for monitoring and managing water-related issues (such as garbage accumulation and industrial waste) using real-time data and computer vision.

## Project Structure

### 1. Smartwater (Mobile App & Admin Dashboard)
The core frontend and admin applications located in the `Smartwater` directory.
- **Mobile Application**: Built with **Flutter**, it features user authentication (Google Sign-In), location tracking (Geolocator), image capturing for reporting, and push notifications.
- **Backend & Cloud**: Heavily integrated with Firebase (Auth, Firestore, Cloud Messaging).
- **AI/Machine Learning**: Utilizes custom-trained YOLOv8 models (`yolov8_custom_trained_v2.pt`) for detecting specific water problems (like garbage) directly from images.
- **Admin Tools**: Contains sub-projects for admin management (`admin-dashboard-frontend` and `admin-dashboard-services`), along with Kubernetes manifests for deployment.

### 2. RabbitMqMetrics
Handles the system's message brokering and metrics tracking.
- Uses **RabbitMQ** (integrated into the Flutter app via `dart_amqp`) to handle asynchronous message queues.
- Contains deployment configurations for both **Cloud** and **Local** environments.

## Technologies Used
- **Frontend**: Flutter, Dart
- **Backend**: Firebase, Node.js (Admin Services)
- **Machine Learning**: PyTorch, YOLOv8
- **Messaging/Metrics**: RabbitMQ
- **Deployment**: Kubernetes, Docker
