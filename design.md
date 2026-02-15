# Sahaaya AI – System Design Document

## 1. Introduction
This document describes the architecture and design of Sahaaya AI, an intelligent platform for providing public service access.

---

## 2. System Architecture

### High-Level Architecture

User → Web/Mobile App → API Gateway → Backend Server → AI Services → Database → Cloud Storage

---

## 3. Module Design

### 3.1 User Module
- Registration
- Login
- Profile Management

### 3.2 Chatbot Module
- Natural Language Processing
- Query Handling
- Response Generation

### 3.3 Scheme Recommendation Module
- User Data Analysis
- Eligibility Check
- Scheme Matching

### 3.4 Document Processing Module
- Upload Service
- OCR Processing
- Data Extraction

### 3.5 Admin Module
- Data Management
- User Monitoring
- Report Generation

---

## 4. Database Design

### Collections / Tables

#### Users
- user_id
- name
- email
- language
- location

#### Schemes
- scheme_id
- scheme_name
- eligibility
- benefits

#### Documents
- doc_id
- user_id
- file_url
- extracted_text

---

## 5. Data Flow Design

1. User submits query
2. Backend receives request
3. AI model processes input
4. Database fetches data
5. Response sent to user

---

## 6. API Design

| Endpoint | Method | Purpose |
|----------|--------|---------|
| /login | POST | User login |
| /chat | POST | Chatbot query |
| /upload | POST | Document upload |
| /schemes | GET | Fetch schemes |

---

## 7. Security Design

- JWT Authentication
- Encrypted Storage
- Secure APIs
- Access Control

---

## 8. Deployment Design

- Frontend → AWS S3
- Backend → AWS Lambda
- Database → Firebase
- Storage → AWS S3

---

## 9. Scalability Design

- Auto Scaling
- Load Balancing
- Microservices
- Caching

---

## 10. Future Enhancements

- Mobile App Version
- Offline Support
- AI Voice Bot
- Government Integration APIs
