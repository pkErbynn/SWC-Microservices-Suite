# SWC Team Management System Microservices Suite

This project is a microservices-based Team Management System built with ASP.NET Core, utilizing Event Sourcing (ES) and Command Query Responsibility Segregation (CQRS) patterns to streamline team operations.

For companies with geographically distributed teams, keeping track of members — monitoring their locations, managing contact information, and assigning projects — can be challenging. 

This system addresses these challenges by providing a comprehensive solution for real-time location tracking, proximity detection, and effective team management. It empowers clients to manage team lists and member details effortlessly, ensuring smooth coordination and communication across the organization.


This cutting-edge suite of scalable, event-driven microservices for team management enables resilient inter-service communication and real-time data processing, further enhancing operational efficiency.

### Core Technologies Utilized:
- **RabbitMQ** as messaging queue, 
- **PubNub** for realtime messaging, 
- **Redis** as cache, and 
- **C# .NET** as core language
- Asp.Net Web API
- PostgreSQL
- InMemoryDB 
- Entity Framework Core ORM
- Moq Testing Framework
- Docker Desktop
- SwaggerUI / Postman
- Git and GitHub 
- GitHub Actions CI/CD
- Visual Studio Code
- MacOS


### High-Level Architecture:

![Architecture](./project-architecture.png)



### The 6 Microservices Components:

1. [Team Service](https://github.com/pkErbynn/StatlerWaldorfCorp.TeamService)
2. [Location Service](https://github.com/pkErbynn/StatlerWaldorfCorp.LocationService)
3. [Location Reporter](https://github.com/pkErbynn/StatlerWaldorfCorp.ES-CQRS-LocationReporter)
4. [Event Processor](https://github.com/pkErbynn/StatlerWaldorfCorp.ES-CQRS-EventProcessor)
5. [Proximity Monitor](https://github.com/pkErbynn/StatlerWaldorfCorp.ES-CQRS-ProximityMonitor)
6. [Reality Consumer](https://github.com/pkErbynn/StatlerWaldorfCorp.ES-CQRS-RealityConsumer)

---

#### 1. Team Service
- **Repository:** [StatlerWaldorfCorp.TeamService](https://github.com/pkErbynn/StatlerWaldorfCorp.TeamService)
- **Description:** This microservice manages team-related operations, including maintaining team lists, handling member details, and overseeing project assignments. This microservice ensures effective team management and coordination.

### 2. Location Service
- **Repository:** [StatlerWaldorfCorp.LocationService](https://github.com/pkErbynn/StatlerWaldorfCorp.LocationService)
- **Description:** This microservice provides comprehensive location-based services and APIs. It manages historical location data and facilitates queries related to team member locations.

### 3. Location Reporter
- **Repository:** [StatlerWaldorfCorp.ES-CQRS-LocationReporter](https://github.com/pkErbynn/StatlerWaldorfCorp.ES-CQRS-LocationReporter)
- **Description:** This microservice facilitates real-time reporting of device locations. It handles incoming location data and updates the system with the latest location information.

### 4. Event Processor
- **Repository:** [StatlerWaldorfCorp.ES-CQRS-EventProcessor](https://github.com/pkErbynn/StatlerWaldorfCorp.ES-CQRS-EventProcessor)
- **Description:** This microservice is responsible for processing and handling events using CQRS (Command Query Responsibility Segregation) principles. It processes inbound events, performs the necessary operations, and manages event streams efficiently.

### 5. Proximity Monitor
- **Repository:** [StatlerWaldorfCorp.ES-CQRS-ProximityMonitor](https://github.com/pkErbynn/StatlerWaldorfCorp.ES-CQRS-ProximityMonitor)
- **Description:** This microservice monitors and analyzes proximity events between devices. This microservice triggers real-time alerts and notifications based on detected proximity conditions.

### 6. Reality Consumer
- **Repository:** [StatlerWaldorfCorp.ES-CQRS-RealityConsumer](https://github.com/pkErbynn/StatlerWaldorfCorp.ES-CQRS-RealityConsumer)
- **Description:** This microservice consumes and processes reality events from the event stream. This microservice is responsible for transforming and utilizing these events for further application logic and data processing.

