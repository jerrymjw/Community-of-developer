# What is API testing? Can you explain with an example?

[What is API testing? Can you explain with an example?](https://www.quora.com/What-is-API-testing-Can-you-explain-with-an-example)

In simple terms, API testing is intended to reveal bugs, inconsistencies or deviations from the expected behavior of an API. Commonly, applications have three separate layers:

Presentation Layer or user interface
Business Layer or application user interface for business logic processing
Database Layer for modeling and manipulating data
API testing is performed at the most critical layer of software architecture, the Business Layer. It is in the business layer, business logic processing is carried out, and all transactions between User Interface(UI) and database happen. So, making sure that, API offers complete intended functionality allows for easy future expansion of the software product.

You can attend a webinar this week that will explain API testing and Mocking.

For example, viewing API traffic between microservices is essential if you want to understand the root cause of problems found in complex distributed systems.

With Mizu, viewing traffic is easy and quick. You can view all of the API calls that are part of the communication between microservices in Kubernetes the same way you would have used Google Chrome Dev Tool to view the traffic of your webapps.

![What is API testing](/Users/jerry/Desktop/IT社区/Community-of-developer/picture/What is API testing?.jpeg)

**No Installation Necessary: No Code instrumentation and not a proxy**

Mizu works by injecting a container that performs a tcpdump-like operation at the node level of a Kubernetes cluster. This operation can be performed on-demand via a CLI that injects the container when run. Alternatively, when ^C is used, it removes the container.

Otherwise, Mizu passively observes traffic at the network level and is not a proxy.

Mizu doesn’t require code instrumentation. It can be used in true on-demand fashion without prior preparation.

**Simple-yet-powerful CLI**

**Mizu uses Kubectl**

The CLI is built in Golang, and can be downloaded and run without installation. Mizu uses kubectl, and can therefore run on any node through which kubectl is configured.

**Use Regular Expression to Qualify Pods to Observe**

While you can simply observe all traffic, you can also qualify specific pods to observe through a regular expression. This allows you to capture traffic from multiple pods as well as pods that don't exist yet. As long as Mizu is operational, pods with names that match the regular expression will be observed, and their traffic logged. This is especially good when pod deployment is dynamic and ever-changing (when pods go up, pods go down).