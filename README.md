## Assignment in Advanced Systems Integration & Architecture
1. Define Service Oriented Architecture(SOA).
- Service-oriented architecture (SOA) is an enterprise-wide approach to software development that takes 
advantage of reusable software components, or services. Each service is comprised of the code and data 
integrations required to execute a specific business function—for example, checking a customer’s credit, 
signing in to a website, or processing a mortgage application.

2. List and discuss the characteristics of SOA.
- Standardized Service Contracts: Services adhere to a service description.
- Loose Coupling: Services minimize dependencies on each other and create specific types of relationships within and outside of 
service boundaries with a constant emphasis on reducing dependencies between service contract, service implementation, and service consumers.
- Abstraction: Services hide the logic they encapsulate from the outside world. 
- Service Reusability: Logic is divided into services with the intent of maximizing reuse.
- Autonomy: Services should have control over the logic they encapsulate.
- Statelessness: Incorporate state management deferral extensions within a service design goal.
- Discoverability: Services can be discovered (usually in a service registry).
- Composability: Services break big problems into little problems. This is elated to the Reusability principle.
- Interoperability: Services should use standards that allow diverse subscribers to use the service.


3. Define Microservices.
- Microservices are a true cloud-native architectural approach, and by using them, teams can update code more easily, use different 
stacks for different components, and scale the component independently of one another, reducing the waste and cost 
associated with having to scale entire applications because a single feature might be facing too much load

4. List and discuss the benefits of using Microservices.
- Independently deployable: Perhaps the single most important characteristic of microservices is that because the services are smaller and 
independently deployable Microservices promise organizations an antidote to the visceral frustrations associated with small changes taking huge amounts of time. 
- Right tool for the job: In traditional n-tier architecture patterns, an application typically shares a common stack, with a large, relational
database supporting the entire application. This approach has several obvious drawbacks—the most significant of which is that every component 
of an application must share a common stack, data model, and database, even if there is a clear, better tool for the job for certain elements. 
- Precise scaling: With microservices, individual services can be individually 
deployed—but they can be individually scaled, as well. The resulting benefit is obvious: Done correctly, microservices 
require less infrastructure than monolithic applications because they enable precise scaling of only the components 
that require it, instead of the entire application in the case of monolithic applications.

5. List and discuss the similarities and differences of SOA and Microservices.
DIFFERENCE
- Reuse: In SOA, reusability of integrations is the primary goal, and at an enterprise level, striving for some level of reuse is essential. 
Reusability and component sharing in an SOA architecture increases scalability and efficiency.
In microservices architecture, creating a microservices component that is reused at runtime throughout an application results in dependencies that reduce agility and resilience. 
Microservices components generally prefer to reuse code by copying and accepting data duplication to help improve decoupling.
- Synchronous calls
The reusable services in SOA are available across the enterprise using predominantly synchronous protocols like RESTful APIs.
However, within a microservice application, synchronous calls introduce real-time dependencies, resulting in a loss of resilience. 
These dependencies may also cause latency, which impacts performance. Within a microservices application, 
interaction patterns based on asynchronous communication are preferred, such as event sourcing, 
in which a publish/subscribe model is used to enable a microservices component to remain up to date on changes happening to the data in another component.
- Data duplication
A clear aim of providing services in an SOA is for all applications to synchronously obtain and 
alter data directly at its primary source, which reduces the need to maintain complex data synchronization patterns.
In microservices applications, ideally, each microservice has local access to all the data it needs to ensure its independence from other microservices 
and indeed from other applications — even if this means some duplication of data in other systems. Of course, this duplication adds complexity, 
so it must be balanced against the gains in agility and performance, but this is accepted as a reality of microservices design.

SIMILARITIES
- Both are collections that focus on performing specific functions.
- Both are smaller in overall scope than one large monolithic architecture.
- Both require decentralization in the internal culture with cross-functional collaborative abilities.
- Both allow the choice of program languages that best suit each service.
