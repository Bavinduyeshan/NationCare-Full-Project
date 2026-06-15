🏥 NationCare – National Healthcare Management Platform

NationCare is a nationwide, cloud-native, microservices-based healthcare platform designed to unify and modernize healthcare systems across multiple hospitals and healthcare providers.

It is the next-generation evolution of Vitalix, redesigned for enterprise-scale deployment, high availability, and national interoperability.

🚀 Overview

NationCare digitizes and centralizes healthcare operations to solve real-world problems such as:

Fragmented patient records across hospitals
Manual appointment and scheduling systems
Lack of real-time communication between healthcare actors
Inefficient administrative monitoring and reporting

The system provides a unified ecosystem for:

👨‍⚕️ Doctors
🧑‍🤝‍🧑 Patients
🏥 Hospitals
🛡️ Administrators
🎯 Core Vision

To build a national digital healthcare backbone enabling:

Seamless cross-hospital patient access
Real-time clinical data sharing
Secure and scalable healthcare workflows
Data-driven medical decision-making
Fully interoperable hospital systems
🏗️ System Architecture

NationCare follows a microservices architecture with centralized routing and service discovery.

🔗 Core Infrastructure
🌐 API Gateway – Single entry point for all requests
🧭 Eureka Server – Service discovery and load balancing
🔐 JWT Authentication – Secure access control
⚡ OpenFeign – Inter-service communication
🐘 PostgreSQL – Distributed database per service
🧩 Microservices Architecture

Each service is independently deployable and responsible for a specific business domain.

🔐 User Service

Handles authentication, authorization, and role management.

User registration and login
JWT token generation
Role-based access control (Admin / Doctor / Patient)
🧑 Patient Service

Responsible for managing all patient-related data and identity operations.

📌 Responsibilities
Patient registration and onboarding
Patient profile management
Patient identity and medical linking
🔳 QR Code Feature (Inside Patient Service)

QR functionality is implemented inside the Patient Service as internal methods, not as a separate microservice.

⚙️ QR Operations
generatePatientQr(patientId)
createQrPayload(patient)
decodeQrData(qrData)
📱 Flow
Patient is registered in Patient Service
Unique patient ID (UUID) is generated
QR code is generated from patient identity
QR is scanned at hospital entry
Patient data is fetched instantly
👨‍⚕️ Doctor Service

Manages doctor profiles, availability, and assignments.

📅 Appointment Service

Handles scheduling and appointment lifecycle management.

Booking / rescheduling / cancellation
Doctor-patient scheduling system
🩺 Medical Records Service

Stores and manages clinical data.

Diagnoses
Prescriptions
Medical history
Treatment records
🔔 Notification Service

Handles system-wide notifications.

Email notifications
SMS alerts
Appointment reminders
System alerts
📊 Report Service

Generates analytics and downloadable reports.

PDF / CSV report generation
Hospital analytics
Patient summaries
🧾 Audit Service

Tracks system activity for security and compliance.

User activity logs
API access tracking
Audit trails
🌐 Infrastructure Services
🌐 API Gateway
Central entry point for all requests
Request routing and filtering
Security enforcement
🧭 Eureka Server
Service registration
Load balancing
Service discovery
🧠 Architecture Diagram
                          🌐 API GATEWAY
                                 |
     ---------------------------------------------------------
     |        |          |           |          |            |
 User   Patient   Doctor   Appointment   Medical Records   Notification
                                 |
                         🧾 Audit Service
                                 |
                         📊 Report Service
                                 |
                         🧭 Eureka Server
🛠️ Tech Stack
Backend
☕ Spring Boot (Microservices)
🌩 Spring Cloud Gateway
🧭 Netflix Eureka
🔗 OpenFeign
🔐 Spring Security + JWT
Database
🐘 PostgreSQL (per-service database)
Frontend
⚛️ React (Vite)
🎨 Tailwind CSS
📦 TypeScript
Architecture
Microservices architecture
Cloud-native design
REST-based communication
🔐 Security
JWT-based authentication
Role-based access control (RBAC)
API Gateway security filtering
Secure inter-service communication
Audit logging for compliance
⚙️ Key Features
🏥 Healthcare System
Unified patient records across hospitals
Doctor scheduling system
Cross-hospital data access
📡 Real-Time Operations
Instant notifications
Live appointment updates
Fast QR-based patient lookup
📊 Analytics
Hospital performance dashboards
Patient health insights
Administrative reporting
🧾 Compliance
Full audit tracking
Secure system logs
Healthcare-grade traceability
🔗 Repository Structure
🖥️ Frontend Applications
🧑 Patient Portal → https://github.com/your-username/patient-frontend
👨‍⚕️ Doctor Portal → https://github.com/your-username/doctor-frontend
⚙️ Backend Microservices
🔐 User Service → https://github.com/your-username/user-service
🧑 Patient Service → https://github.com/your-username/patient-service
👨‍⚕️ Doctor Service → https://github.com/your-username/doctor-service
📅 Appointment Service → https://github.com/your-username/appointment-service
🩺 Medical Records Service → https://github.com/your-username/medical-records-service
🔔 Notification Service → https://github.com/your-username/notification-service
🧾 Audit Service → https://github.com/your-username/audit-service
📊 Report Service → https://github.com/your-username/report-service
🧠 Infrastructure
🌐 API Gateway → https://github.com/your-username/api-gateway
🧭 Eureka Server → https://github.com/your-username/eureka-server
🚀 Deployment Strategy
Docker containerized microservices
Kubernetes-ready architecture
Load-balanced API Gateway
Horizontal scaling support
Centralized logging (optional ELK stack)
🔮 Future Enhancements
📱 Mobile apps (Patient & Doctor)
🤖 AI-assisted diagnosis system
🧠 Predictive healthcare analytics
💬 Real-time chat system
☁️ Cloud deployment (AWS / Azure / GCP)
🏥 Multi-tenant hospital SaaS model
📌 Project Status

🚧 Active Development – Enterprise Scaling Phase

👨‍💻 Author

Built by Bavindu Yeshan
🚀 From Vitalix → NationCare (National Healthcare Platform Evolution)

⭐ Why NationCare Matters

NationCare is a real-world enterprise-grade healthcare architecture simulation, designed with:

Scalable microservices design
Real hospital workflows
Secure distributed systems
Production-ready architecture patterns
