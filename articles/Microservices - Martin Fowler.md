

The microservice architecture style is an approach to developing a single application as a suite of small services, each running in its own process and communicating with lightweigh mechanisms. These services are built around business capabilities and independently deployable by fully automated machinery.



# Characteristics of a Microservice Architecture

### Componentization via Services:

**Component** is a unit of software that is independently replaceable and upgradeable.

Microservices will use libraries, but their primary way of componentizing their own software is by breaking down into services. **Libraries** are components that are linked into a program and called using in-memory function calls, while **services** are out-of-process components who communicate with a mechanism such as web service reques, or remote procedure call.

Benefits of using services as components:
- Services are independently deployable, no need to redeploy the application every time a component is modified, only the component's service need to be deployed.
- More explicit component interface

Downsides:
- Remote calls are more expensive than in process calls


### Organized around Business Capabilities

When looking to split a large application into parts, often management focuses on the technology layer, leading to UI teams, server-side logic teams, and database teams. When teams are separated along these lines, even simple changes can lead to a cross-team project taking time and budgetary approval.

The microservice approach to division:

- Services are organized around Business Capabilities, in other words, a service is responsible for one business area, including user-interface, persistant storage, and any external colaboration .
- Cross-functional teams, including the full range of skills required for the development: user-experience, database, and project management.  Each team takes care of one service.


### Products not Projects

A team should own a product over its full lifetime *(Amazon's notion of **"[you build, you run it](https://queue.acm.org/detail.cfm?id=1142065)"**)*, where a development team takes full responsibility for the software in production. This brings developers into day-to-day contact with how their software behaves in production.

Rather than looking at the software as a set of functionality to be completed, there is an on-going relationship where the question is how can software assist its user to enhance the business capability.

The same approach can be done with monolithic application.


### Smart endpoints and dumb pipes

Microservice teams use the principles and protocols that the world wide web is built on. Often used resources can be cached with very little effort on the part of developers.

The second approach in common use is messaging over a lightweigh message bus. The infrastructure chosen is typically dumb (acts as a message router only), the smarts still live in the end points that are producing and consuming messages.


### Decentralized Governance

Each microservice can use different tools and technologies for different types of problems - not every problem is a nail and not every solution a hammer.

Splitting the monolith's components out into services we have a choice when building each of them. Teams building microservices prefer a different approach to standards too.

Netflix is a good example of an organisation that follows this philosophy. Sharing useful and, above all, battle-tested code as libraries encourages other developers to solve similar problems in similar ways yet leaves the door open to picking a different approach if required.

### Decentralized Data Management

### Infrastructure Automation

### Design for failure

### Evolutionary Design

