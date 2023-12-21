# Part 2: Microservices Architecture

## Q1: Define what is a Microservices architecture and how does it differ from a Monolithic application.
Microservices is a type of application architecture in which there are several independent services that communicate via APIs.
For example, if you have a website where you can shop online, the shopping basket will be a microservice, the history will be another ... and so on.

Initially, applications had a monolithic architecture, meaning that all the functions and services of an application were locked together and operated as a single unit.
When the application needs to be enhanced, the architecture becomes more complex because the functions are not independent.

In microservices architectures, applications are built so that each core function of the application operates independently. This allows services to be updated without disrupting the application as a whole.

## Q2: Compare Microservices and Monolithic architectures by listing their respective pros and cons.
### Monolithic :
#### PROS :
- Monolithic architectures are generally simpler to develop and deploy, as they have less infrastructure and the architecture is less complex.
#### CONS :
- More difficult to make code changes
- More difficult to make updates or new features without affecting the whole system.
- System testing, debugging and maintenance can be more difficult.
### Microservices :
#### PROS :
- Code can be easily updated and new features and functionality deployed without affecting the entire application.
- You can work independently.
- Components can be scaled independently of each other without the need to scale the whole application.
#### CONS :
- Increased maintenance costs 
- Organizational complexity and Coordination complexity
- Risk of failure cascades

## Q3: In a Micoservices architecture, explain how should the application be split and why.
In a microservices architecture, the application is divided according to the services it offers.
Each microservice must be designed to manage a specific business function and must have a well-defined API for communicating with the other services. This approach enables each microservice to be developed, deployed and scaled independently. The aim is to create a modular, loosely coupled system where changes to one service have no impact on the others, promoting flexibility and maintainability.

## Q4: Briefly explain the CAP theorem and its relevance to distributed systems and Microservices.
The CAP theorem states that in a distributed computer system, it is impossible to simultaneously guarantee consistency, availability and partition tolerance. It suggests that when designing a distributed database, it is only possible to achieve two of these three properties.

In a microservices architecture, the CAP theorem is relevant because microservices often operate in a distributed environment where network partitions can occur. Architects must make trade-offs between consistency and availability to ensure system resilience in the face of network failures.

## Q5: What consequences on the architecture ?

The CAP theorem has consequences. It is important to take care on design systems to prioritize consistency or availability based on the specific requirements of the application. In a microservices, this may involve choosing the right data storage mechanisms, designing resilient communication protocols, and implementing strategies for handling partition scenarios.

## Q6: Provide an example of how microservices can enhance scalability in a cloud environment.
In a cloud environment, microservices can improve scalability by enabling independent scaling of services according to demand.
If we take again the exemple of website where you can shop online:the application with separate microservices for user authentication, the and history. During peak periods, the basket service can be scaled horizontally to cope with increased load without affecting the authentication or history services. This fine-grained scalability ensures efficient use of resources and cost-effectiveness.

## Q7: What is statelessness and why is it important in microservices archi-tecture ?
Stateless microservices do not retain any state or store session-specific data between requests. Each request received by a stateless microservice is processed independently, without relying on previous interactions.
This allows them to be scaled across multiple instances without any impact on their functionality.

## Q8: What purposes does an API Gateway serve ?
API gateways act as a single point of entry for processing all API requests. Its features include traffic management, security protocols, caching and monitoring, enabling APIs to be efficiently managed, optimised and protected.



