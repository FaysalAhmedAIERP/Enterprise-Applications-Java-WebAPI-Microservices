# Enterprise Applications – Java, Web API, Microservices & Cloud Lab

Hands-on enterprise application project covering Java web development, Apache Tomcat deployment, Web API integration, monolithic and microservices architecture, Twelve-Factor App principles, containerized architecture, cloud computing, DDoS resilience, AWS SQS and AWS SNS.

---

## Project Overview

This repository documents a complete practical learning project for Enterprise Applications.

The project was developed and documented using IntelliJ IDEA and covers eight tutorials ranging from enterprise application fundamentals to Java web deployment, Web APIs, microservices, cloud computing, cybersecurity resilience, and AWS messaging architecture.

The main purpose of this repository is to demonstrate practical understanding of modern enterprise application development concepts that can also be applied to ERP software design and development.

---

# Tutorial 1 – Enterprise Application Fundamentals

## Topics Covered

- Enterprise Applications
- Three-Tier Architecture
- Enterprise Design Patterns
- Java Enterprise Technologies
- JSP and Servlet Concepts

## Key Learning

An enterprise application is a large-scale software system designed to support business processes, data, users, and integration requirements.

A typical three-tier enterprise architecture contains:

Presentation Layer
↓
Business / Application Layer
↓
Database / Data Layer

Example:

Web Browser
↓
Java / Tomcat Application
↓
Relational Database

## ERP Relevance

These concepts are directly useful when designing ERP systems where:

- Frontend handles user interaction
- Business layer processes ERP rules
- Database stores procurement, inventory, finance, HR, and sales data

## Evidence File

tutorial1_summary.txt

---

# Tutorial 2 – Java Web Application, Gradle, Tomcat & JSP

## Practical Work Completed

- Configured Java Development Kit
- Configured Gradle
- Resolved Gradle/JVM compatibility issue
- Installed Apache Tomcat 10.1
- Configured Tomcat inside IntelliJ IDEA
- Created Tomcat Run Configuration
- Configured HTTP port 8080
- Configured deployment artifact
- Created JSP page
- Built the application successfully
- Deployed the application
- Executed the JSP application successfully in a browser

## Test URL

http://localhost:8080/Web1/hello.jsp

## Successful Output

Hello World

My first JSP page is running on Apache Tomcat.

## Practical Learning

Java Setup
↓
Gradle Build
↓
Tomcat Configuration
↓
JSP Deployment
↓
Browser Execution

## ERP Relevance

The same development flow can be used for:

- ERP web modules
- Procurement systems
- Inventory systems
- Internal enterprise portals
- Java-based business applications

## Evidence File

tutorial2_practical_evidence.txt

---

# Tutorial 3 – Web API Design and Live API Testing

## Topics Covered

- Web API Resources
- HTTP GET
- HTTP POST
- HTTP PUT
- HTTP PATCH
- HTTP DELETE
- JSON
- XML
- REST API endpoints
- Live API testing

## Live API Request

GET https://api.weather.gov/points/38.8894,-77.0352

User-Agent: CT066-Student-Lab

Accept: application/geo+json

## Result

HTTP Status: 200 OK

## API Endpoints Explored

Forecast:
https://api.weather.gov/gridpoints/LWX/97,71/forecast

Hourly Forecast:
https://api.weather.gov/gridpoints/LWX/97,71/forecast/hourly

Forecast Grid Data:
https://api.weather.gov/gridpoints/LWX/97,71

Observation Stations:
https://api.weather.gov/gridpoints/LWX/97,71/stations

Alerts:
https://api.weather.gov/alerts/active

## ERP Relevance

Web APIs are important in ERP systems for integration with:

- Suppliers
- Logistics providers
- Banks
- Payment gateways
- Government systems
- Mobile applications
- External business platforms

## Evidence Files

web_api_notes.txt  
weather_api.http  
weather_endpoints.txt

---

# Tutorial 4 – Monolithic vs Microservices Architecture

## Topics Covered

- Monolithic Applications
- Microservices
- API Throttling
- Metering
- Continuous Delivery
- Continuous Deployment
- Change Request Lifecycle

## Monolithic Architecture

Web Client
↓
Single Enterprise Application
↓
Login
Customer
Inventory
Order
Payment
Reporting
↓
Shared Database

## Microservices Architecture

Web / Mobile Client
↓
API Gateway / Load Balancer
↓
Auth Service
Order Service
Inventory Service
Payment Service
Reporting Service
↓
Independent Databases

## ERP Relevance

A large ERP system can be separated into independent services such as:

- Procurement Service
- Inventory Service
- Finance Service
- HR Service
- Sales Service
- Supplier Service
- Reporting Service

## Evidence Files

monolithic_microservices.txt  
architecture.txt  
login_change_pipeline.txt

---

# Tutorial 5 – Twelve-Factor Application

## Objective

The Movie Microservice was assessed using Twelve-Factor App principles.

## Twelve Factors

1. Codebase
2. Dependencies
3. Config
4. Backing Services
5. Build, Release, Run
6. Processes
7. Port Binding
8. Concurrency
9. Disposability
10. Dev/Prod Parity
11. Logs
12. Admin Processes

## Example Architecture

Client
↓
REST API Controller
↓
Movie Service
↓
Repository Layer
↓
Persistent Datastore

## ERP Relevance

Twelve-Factor principles help make ERP applications:

- Cloud ready
- Scalable
- Configurable
- Maintainable
- Easier to deploy
- Easier to monitor

## Evidence Files

twelve_factor_assessment.txt  
movie_microservice_architecture.txt  
twelve_factor_summary.txt

---

# Tutorial 6 – Containerized Pet Clinic Microservices Architecture

## Objective

The original monolithic Pet Clinic application was redesigned conceptually as a containerized microservices architecture.

## Services Designed

- Owner Service
- Pet Service
- Vet Service
- Visit Service

## Architecture

Web Browser / Client
↓
Load Balancer / API Gateway
↓
Owner Service
Pet Service
Vet Service
Visit Service
↓
Independent Databases

## Supporting Components

- Service Discovery
- Centralized Configuration
- Centralized Logging
- Monitoring
- Health Checks
- Container Platform
- Kubernetes Concepts
- Load Balancing
- Scaling
- Rolling Deployment

## ERP Relevance

This same architecture can be used to separate ERP modules into independently deployable services.

## Evidence Files

pet_clinic_architecture.txt  
architecture_explanation.txt  
component_mapping.txt

---

# Tutorial 7 – Cloud Computing, Multi-Cloud & Multi-CDN

## Cloud Computing Models

### IaaS – Infrastructure as a Service

Provides:

- Virtual machines
- Storage
- Networking

Examples:

- AWS EC2
- Azure Virtual Machines

### PaaS – Platform as a Service

Provides managed application development and deployment platforms.

Examples:

- Google App Engine
- Azure App Service

### SaaS – Software as a Service

Provides complete software applications over the internet.

Examples:

- Microsoft 365
- Salesforce

### Serverless / FaaS

Runs functions on demand without directly managing servers.

Example:

- AWS Lambda

## Multi-Cloud

Multi-Cloud means using more than one cloud provider.

Example:

AWS  
+ Microsoft Azure  
+ Google Cloud

Benefits:

- Reduced vendor dependency
- Higher resilience
- Access to specialized cloud services
- Better workload placement

## Multi-CDN

Multi-CDN means using multiple Content Delivery Network providers.

Benefits:

- Better global performance
- Automatic failover
- Higher availability
- Geographic optimization
- Reduced dependency on one provider

## ERP Relevance

Cloud architecture can support:

- Cloud ERP
- Global branch access
- Disaster recovery
- High availability
- Business continuity
- Regional deployment

## Evidence Files

cloud_computing.txt  
multi_cloud.txt  
multi_cdn.txt

---

# Tutorial 8 – DDoS, AWS SQS & AWS SNS

## Part A – DDoS Security

Topics covered:

- Distributed Denial-of-Service attacks
- Volumetric attacks
- Protocol attacks
- Application-layer attacks
- Business impact
- DDoS protection
- CDN
- Web Application Firewall
- Rate Limiting
- API Throttling
- Traffic Scrubbing
- Load Balancing
- Monitoring
- Incident Response

## DDoS Defence Architecture

Internet Traffic
↓
DDoS Protection / Traffic Scrubbing
↓
CDN + Web Application Firewall
↓
API Gateway / Rate Limiting
↓
Load Balancer
↓
Application Instances
↓
Database

## Part B – AWS SQS

AWS SQS was studied in the context of a connected-car application.

Architecture:

Connected Car / Sensors
↓
API / Data Ingestion
↓
AWS SQS Queue
↓
Map Worker / Analytics Worker
↓
RDS / DynamoDB / S3

## SQS Concepts Covered

- Producer
- Consumer
- Message Queue
- Asynchronous Processing
- Message Buffering
- Visibility Timeout
- Retry
- Dead-Letter Queue
- Message Retention
- Standard Queue
- FIFO Queue
- Independent Scaling

## Part C – AWS SNS

AWS SNS was studied as a publish/subscribe messaging system.

Architecture:

Publisher
↓
SNS Topic
↓
Multiple Subscribers

## SQS vs SNS

SQS = Queue-based asynchronous processing

SNS = Publish/Subscribe event broadcasting

## Combined SNS + SQS Architecture

Connected Car Event
↓
AWS SNS
↓
SQS A / SQS B
↓
Map Service / Analytics Service

## ERP Relevance

SQS and SNS can be used in ERP systems for:

- Background jobs
- Purchase Order processing
- Approval workflows
- Inventory updates
- Event-driven notifications
- Supplier integration
- System alerts
- Asynchronous data processing

## Evidence Files

ddos_security.txt  
aws_sqs.txt  
sqs_vs_sns.txt

---

# Complete Tutorial Summary

This repository contains work from all eight tutorials:

Tutorial 1  
Enterprise Application Fundamentals

Tutorial 2  
Java + Gradle + Apache Tomcat + JSP

Tutorial 3  
Web API + HTTP Methods + JSON/XML + Live API Testing

Tutorial 4  
Monolithic vs Microservices + CI/CD Concepts

Tutorial 5  
Twelve-Factor Application

Tutorial 6  
Containerized Microservices + Load Balancing + Kubernetes Concepts

Tutorial 7  
Cloud + Multi-Cloud + Multi-CDN

Tutorial 8  
DDoS Security + AWS SQS + AWS SNS

---

# Enterprise / ERP Software Application

The knowledge from these tutorials can be combined into a modern ERP architecture.

User / Web Interface
↓
API Gateway
↓
Procurement Service
Inventory Service
Finance Service
HR Service
Sales Service
↓
Independent Databases
↓
Messaging / Events
↓
AWS SQS / AWS SNS

Possible ERP applications include:

- Procurement Management
- Purchase Requisition
- Purchase Order Processing
- Supplier Management
- Inventory Management
- Warehouse Management
- Finance Integration
- HR Management
- Sales Management
- Order Processing
- API Integration
- Business Process Automation
- Cloud ERP Deployment
- Event-Driven Notifications
- Cybersecurity and Availability Engineering

---

# Practical Outcomes

Through this project I practiced:

- Java development environment setup
- Gradle configuration
- Apache Tomcat configuration
- JSP deployment
- Web application execution
- REST API requests
- HTTP response validation
- API endpoint analysis
- Enterprise architecture modelling
- Microservices design
- Twelve-Factor methodology
- Containerized architecture concepts
- Cloud computing architecture
- DDoS resilience
- AWS SQS
- AWS SNS
- ERP architecture mapping

---

# Tools & Technologies

- Java 17
- IntelliJ IDEA
- Gradle
- Apache Tomcat 10.1
- JSP
- HTML
- REST API
- HTTP
- JSON
- XML
- Microservices
- Twelve-Factor App
- Cloud Computing
- Containerization
- Kubernetes Concepts
- AWS SQS
- AWS SNS
- DDoS Protection Concepts

---

# Screenshots & Evidence

Practical screenshots are stored in:

/screenshots

The screenshots include:

- Project structure
- Tutorial 1 evidence
- Tutorial 2 practical evidence
- JSP Hello World output
- Web API request
- Architecture exercises
- Twelve-Factor assessment
- Containerized architecture
- Cloud computing exercises
- AWS SQS and SNS work

---

# Repository Structure

Enterprise-Applications-Java-WebAPI-Microservices

- screenshots/
- build.gradle
- settings.gradle
- gradlew
- gradlew.bat
- tutorial1_summary.txt
- tutorial2_practical_evidence.txt
- web_api_notes.txt
- weather_api.http
- weather_endpoints.txt
- architecture.txt
- monolithic_microservices.txt
- login_change_pipeline.txt
- twelve_factor_assessment.txt
- movie_microservice_architecture.txt
- twelve_factor_summary.txt
- pet_clinic_architecture.txt
- architecture_explanation.txt
- component_mapping.txt
- cloud_computing.txt
- multi_cloud.txt
- multi_cdn.txt
- ddos_security.txt
- aws_sqs.txt
- sqs_vs_sns.txt

---

# Key Learning Journey

Enterprise Application Fundamentals  
↓  
Java Web Development  
↓  
Apache Tomcat Deployment  
↓  
Web API Integration  
↓  
Monolithic Architecture  
↓  
Microservices  
↓  
Twelve-Factor Application  
↓  
Containers & Kubernetes Concepts  
↓  
Cloud Computing  
↓  
Cybersecurity Resilience  
↓  
AWS Messaging  
↓  
Modern Enterprise / ERP Architecture

---

# Author

**Faysal Ahmed**

AI, ERP, Supply Chain Automation & Cybersecurity Specialist

GitHub: **FaysalAhmedAIERP**
