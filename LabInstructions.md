# 🧪 Lab: Designing Architecture with GitHub Copilot

## **Lab Title:**

**End-to-End Architecture Design Using GitHub Copilot**

## **Lab Duration:**

**90–120 minutes**

## **Lab Objectives**

By the end of this lab, learners will be able to:

* Use GitHub Copilot to analyze system requirements.
* Generate architecture recommendations.
* Create architecture documents (HLD, diagrams, ADR).
* Generate architecture scaffolding for implementation and deployment.
* Understand how Copilot accelerates the architecture workflow.

---

# 🟧 Lab Scenario

You are working as a **Solution Architect** for a new project called **QuickFood**, a food delivery platform similar to Swiggy/Zomato.

The system must support:

* User registration & login
* Restaurant onboarding
* Menu management
* Order placement
* Order tracking with live status
* Payment handling
* Expected scale: **150K daily active users**
* Independent deployments
* High availability

You will use **GitHub Copilot Chat** to:

1. Understand requirements
2. Generate architecture documentation
3. Create code scaffolding for the architecture

---

# 🟩 PART A: Understanding Requirements Using Copilot

## **Task 1: Architecture Recommendation**

### **Prompt:**

```
Given the following requirements:

- A food delivery system with user, restaurant, order, tracking, and payment modules
- Must scale to 150K daily active users
- Requires real-time order tracking
- Teams should deploy modules independently

Recommend the best architecture style. Compare:
- Monolith
- Modular Monolith
- Microservices
- Event-driven Microservices

Provide pros and cons and justify the final choice.
```

### **Student Deliverable:**

* 1–2 paragraph summary of Copilot's suggestion
* State whether you agree with it (Yes/No + Why)

---

# 🟦 PART B: Drafting Architecture Documents Using Copilot

## **Task 2: Generate High-Level Architecture**

### **Prompt:**

```
Create a high-level system architecture for the QuickFood application.
Include the following components:
- User Service
- Restaurant Service
- Menu Service
- Order Service
- Delivery Tracking Service
- Payment Service
- API Gateway
- Event Bus (Kafka/RabbitMQ)

Describe each component and how they interact.
```

---

## **Task 3: Component Diagram (Text-Based)**

### **Prompt:**

```
Create a text-based component diagram for QuickFood architecture using Markdown or ASCII diagram format.
```

---

## **Task 4: Sequence Diagram (PlantUML)**

### **Prompt:**

```
Create a PlantUML sequence diagram for the "Place Order" workflow in QuickFood.
Include:
- User
- API Gateway
- Order Service
- Payment Service
- Restaurant Service
- Delivery Tracking Service
- Event Bus
```

---

## **Task 5: Create an ADR**

### **Prompt:**

```
Write an Architecture Decision Record (ADR) for choosing event-driven microservices over request-response for QuickFood order processing.
Follow ADR template format:
- Title
- Context
- Decision
- Consequences
```

---

# 🟨 PART C: Generating Architecture Scaffolding Using Copilot

## **Task 6: Generate Project Structure**

Choose your preferred language (e.g., .NET/Java/Node.js).

### **Prompt (Example for .NET):**

```
Generate a Clean Architecture folder structure for a .NET microservices-based solution for QuickFood.
Include:
- UserService
- RestaurantService
- OrderService
- PaymentService
- DeliveryService

Each service should include folders:
- API
- Application
- Domain
- Infrastructure
- Tests

Provide basic template files for each layer.
```

### **Prompt (Example for Java Spring Boot):**

```
Generate a microservices folder structure for a Java Spring Boot-based QuickFood system.
Include services:
- user-service
- restaurant-service
- order-service
- payment-service
- delivery-service

For each service include folders:
- src/main/java/com/quickfood/<service>/controller
- src/main/java/com/quickfood/<service>/service
- src/main/java/com/quickfood/<service>/repository
- src/main/java/com/quickfood/<service>/model
- src/main/resources
- src/test/java/com/quickfood/<service>

Generate template classes:
- Controller class
- Service class
- Repository interface
- Model class
- Application main class
```

---

## **Task 7: Generate Deployment Templates (Kubernetes)**

### **Prompt:**

```
Generate Kubernetes manifests for QuickFood Order Service:
- Deployment
- Service (LoadBalancer)
- ConfigMap with environment variables
- Liveness and readiness probes
```

---

# 🎓 Final Submission Requirements

Learners must submit a compressed (.zip) folder including:

### ✔ Architecture Summary (Task 1)

### ✔ Generated Architecture Documents

* High-Level Design (HLD)
* Component Diagram
* Sequence Diagram
* ADR

### ✔ Code Scaffolding

* Folder structure
* Template files

### ✔ Deployment Manifests

---

# 🏆 Learning Outcomes

By completing this lab, learners will be able to:

* Use GitHub Copilot for architectural decision-making
* Produce complete architecture documents
* Create diagrams using PlantUML with AI
* Generate microservices scaffolding efficiently
* Produce Infrastructure-as-Code using Copilot

---
