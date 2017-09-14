# Distributed Enabling Platforms

* Teacher: [Nicola Tonellotto](http://pomino.isti.cnr.it/~khast/)
* CFU: 6
* Period: First semester
* Language: English
* Lectures schedule: Monday 16--18 (L1) and Friday 9--11 (C1).
* Question time: After lectures or by appointment
* Email: nicola [dot] tonellotto [at] isti [dot] cnr [dot] it

## Course Overview

In the last years there have been many interesting developments in data bases, distributed systems and in the ways applications are built on top of them. Large web companies such as Google, Microsoft, Amazon, Facebook, LinkedIn and Twitter collect, organize and exploit huge volumes of data and traffic, forcing them to solve new issues and create new tools that enable them to efficiently handle such scale. In this course, the students will gain practical exposure to the skills, tools, and knowledge needed in building and managing very large scale distributed infrastructures to organize and exploit big data. We will look at examples of successful data systems: technologies that form the foundation of the most important web applications applications, and that have to meet scalability, performance and reliability requirements in production every day.

The main course deals with a set of arguments related to the distributed computing platforms. In this course we will explore the issues in very large scale distributed systems - for example, with hundreds or thousands of nodes - and consider how such systems can be designed and programmed. Most common issues and problems in the design and implementations of such systems will be investigated, and the state-of-the-art solutions available in industry-level distributed platforms will be discussed. Examples include the Grid/Cloud platforms, MapReduce systems, data management platforms such as search system infrastructures (e.g., Web search engines) and data management infrastructures (e.g., distributed data stores).

After the course, the students will be able to:

* understand the typical issues of very large scale distributed systems;
* discuss, analyze and inspect very large scale distributed systems;
* master tools, best practices and common procedures to design, implement and program such systems;
* understand the components of a Web search infrastructures;
* understand the components of a distributed data storage infrastructure;
* collect, represent, organize and manage huge volumes of data;
* process big data to generate new knowledge with the MapReduce paradigm.

[//]: <> (This is also a comment.)

## Recommended prerequisites

* Knowledge in Java programming
* Algorithms
* Basic operating systems
* Personal laptop

## Exam

The exam consists in a final project and an oral test. The final project must be delivered before the oral test takes place.

### Final Project
The topic of the final project can be on anything you wish in the space of distributed enabling platforms. Anything reasonably related to topics that we covered in the course is within scope. For reference, there are three types of projects you might consider:

* Implement a big data algorithm in MapReduce: choose a particular big data algorithm (for processing text, graphs, relational data, etc.) and implement it. Ideally, the implementation does not already exist in a library or open-source package. Since I want you to implement the algorithm from scratch, you must avoid to simply copy existing code.
* Implement a software library including some of the techniques discussed during the course (e.g., logical clocks, query processing algorithms, etc.). Again, the implementation should not already exist, and the library should be self contained, using all software development tools to provide a documented, self-contained software (e.g., documentation, dependencies management, unit testing).
* Implement a software tool including some of the techniques discussed during the course (e.g., text indexer, query processor, URL shortener). The implementation should not already exist, and the tool should be self contained, using all software development tools to provide a documented, self-contained software (e.g., documentation, dependencies management, unit testing).

You may work in groups of up to two, or you can also work by yourself if you wish. The amount of effort devoted to the project should be proportional to the number of people in the team.

When you are ready, send the instructor an email describing what you'd like to work on. I will provide you feedback on appropriateness, scope, etc.

Note that we expect your project to be more than a "toy". To calibrate what we mean by "toy", a project running only locally on your computer is a "toy". during the final project discussion I can ask to install and run a demo of your project on a distributed cluster I will make available for testing purposes.

The deliverable for the final project is a report written in Latex. Use the [ACM Templates](http://www.acm.org/publications/proceedings-template). The contents of the report will of course vary by the topic, but I would expect the following sections:

* description the problem you're tackling and what you're trying to accomplish (introduction, problem statement)
* present existing solutions (background, related work)
* detail how you went about solving the problem (methods, algorithms, implementation details, etc.)
* discuss how well things work (some sort of evaluation and results).

Once again, length would vary, but please does not exceed the 10 pages limit (in the ACM Template).

When your report and software are ready, please put them in a Web repository I can access (Web server, Github, Bitbucket, Google Drive), and expect a couple of emails exchanges and appointments to discuss the project before the oral examination takes place.

### Oral Test
During the oral test you will have to answer queries on your final project and the course topics with the help of a whiteboard.

## Lectures

## Tentative Topics
The following list of topics is subject to change.

| Topic | Description | References |
|--------|-------------|------------|
|Datacenters & Cloud | | [BCH] Chapters 1 and 4 |
| MapReduce Programming Model | | |
| Programming in Hadoop| | |
| Algorithms in MapReduce: | Real-world problems solved with MapReduce: PageRank, Inverted Indexing, Near Duplicate Detection | |
| Data models, representation and storage| | |
| Data management and replication | | |
| Data Consistency & Consensus | Consistency Models, Eventual Consistency, Consensus, FLP and CAP Theorems, PAXOS| |
| Time in distributed System| | |
| Web Serch Engine Infrastructure| Crawling, Indexing, Query Processing||

## References

*  The Datacenter as a Computer, 2nd edition, L.A. Barroso, J. Clidaras, U. Holzle, Morgan & Claypool Publisher, 2013\. ([Amazon](https://www.amazon.com/Datacenter-Computer-Introduction-Warehouse-Scale-Architecture/dp/1627050094)) [BCH]
## Useful Links and Material

The following schedule is subject to change.

| Class    | Topics                           |  Resources | Assignments       |
|----------|----------------------------------|------------| ----------------  |
| Aug 17   | [Core Concepts](http://tiny.cc/CSC-DevOpsCore) |  [Adages](https://github.com/CSC-DevOps/Course/blob/master/Readings/AdagesI.pdf)        | [HW0](https://github.com/CSC-DevOps/Course/blob/master/HW/HW0.md) |
| Aug 22   | [Configuration Management](http://tiny.cc/devops-cm-slides)  |            | |
| Aug 24   | [Workshop: Managed Environments](https://github.com/CSC-DevOps/CM/blob/master/README.md) |            | [HW1](HW/HW1.md) |
| Aug 29   | [Workshop: Ansible](https://github.com/CSC-DevOps/CM/blob/master/README.md) |  |   |
| Aug 31   | Workshop: Provisioning   |            |                   |
| Sep 5    | [Build Management](https://docs.google.com/presentation/d/1PeI-RbsisPtC8tbKMgtB3IDlffLjE6obQkp-tL0Cmsw/edit#slide=id.p)   |             | [MILESTONE: CM+BUILD](Project/CM.md) |
| Sep 7   |  [Workshop: Build Servers](https://github.com/CSC-DevOps/Course/blob/master/Workshops/Build.md)       |            |                   |
| Sep 12   | [Analysis](https://docs.google.com/presentation/d/1EkfcbwXko9gvtel0t4GD_cpE4me-OAIwdYt0p_OAeIs/edit#slide=id.p)                         |            |                   |
| Sep 14   | [Workshop: Complexity](https://github.com/CSC-DevOps/Complexity)                |            |                   |
| Sep 19   | [Test Management](https://docs.google.com/presentation/d/1Wv149dt56DAixTn5BqdyHwVxBWyHU1pk5ohL7jlVAWs/edit#slide=id.p)                  |            | |        
| Sep 21   | [Workshop: Test Suites]()    |      |    |
| Sep 26   | [Workshop: Fuzzing](https://github.com/CSC-DevOps/Fuzzing) |   |   MILESTONE: TEST/ANALYSIS |
| Sep 28   | [Workshop: Test Generation](https://github.com/CSC-DevOps/TestGeneration)   |   |  HW2   |
| Oct 3   |  [Tech Talks #1](https://github.com/CSC-DevOps/Course/blob/master/TechTalks.md)  |     |  |
| Oct 5&mdash;6    | Fall Break                       |            |                   |
| Oct 10   | [Infrastructure Management](https://1drv.ms/p/s!AG169vwdL5H_jUY)        |            |                   |
| Oct 12  |  [Tech Talks #2](https://github.com/CSC-DevOps/Course/blob/master/TechTalks.md)                   |     |                   |
| Oct 17   | [Feature Flags/Property Sets/Redis](https://docs.google.com/presentation/d/1cqVz0H4t-b7ZWMEbfBaYJDLSePhMOOjWW04CRzsIY5k/edit#slide=id.p)|            | MILESTONE: DEPLOY |
| Oct 19   | [Workshop: Queues, Caches, Proxies](https://github.com/CSC-DevOps/Queues)|            | HW3       |            
| Oct 24   | [Staging + Deployment](https://docs.google.com/presentation/d/1J3oDEPSGzDGa0B41Ppe8yA02tYicSgstVXHU5mGxU5w/edit#slide=id.g1da8fd6af9_0_196)             |            |                   |
| Oct 26    | [Workshop: Deployment](https://github.com/CSC-DevOps/Deployment/blob/master/README.md)             |            |                   |
| Oct 31   | [Tech Talks #3](https://github.com/CSC-DevOps/Course/blob/master/TechTalks.md)   |            |                   |
| Nov 2   | [Advanced Docker: Deployment](https://github.com/CSC-DevOps/Course/blob/master/Workshops/AdvancedDocker.md)                    |   | HW4    |
| Nov 7   | [Analysis + Monitoring](https://docs.google.com/presentation/d/1swei7oeXWZGnXe9gC1jlh4Gd1h9Ri6I6x2kTgKr1BVw/edit?usp=sharing)            |            | MILESTONE: SPECIAL|
| Nov 9   | Workshop: Monitoring + Resilience|  [Chaos Engineering](https://www.facebook.com/notes/tpm-networking-group/notes-from-chaos-community-day-nov-4th-2015/1042668315800057)          |                   |
| Nov 14   |  DevOps at Work I   |            |             |
| Nov 16   |  DevOps at Work II  |            |             |
| Nov 21   | [Tech Talks #4](https://github.com/CSC-DevOps/Course/blob/master/TechTalks.md)          |                   |
| Nov 23   | Thanksgiving                     |            |                   |
| Nov 28   | Demos                     |            |                   |
| Nov 30   | Demos                     |            |                   |
| Dec 5   | Exam (1:00PM - 4:00PM)           |            |                   |

### Additional Resources

[Slack](https://cscdevops-fall2017.slack.com)

##### Papers

* [An empirical study on principles and practices of continuous delivery and deployment](https://peerj.com/preprints/1889.pdf)

##### Books

* [Effective DevOps](https://www.amazon.com/Effective-DevOps-Building-Collaboration-Affinity/dp/1491926309)
* [Ansible: Up and Running](http://www.ansiblebook.com/)
* [Continous Delivery](http://continuousdelivery.com/)
* [Continous Integration](http://www.amazon.com/Continuous-Integration-Improving-Software-Reducing/dp/0321336380)
* [Designing Data-Intensive Applications](http://dataintensive.net/)
* [Systems Performance: Enterprise and the Cloud](http://www.brendangregg.com/sysperfbook.html)
* [The Practice of Cloud System Administration](http://the-cloud-book.com/)
* [DevOps: A Software Architect's Perspective, SEI](http://www.amazon.com/DevOps-Software-Architects-Perspective-Engineering/dp/0134049845)

##### Glossary of Tools

* [http://newrelic.com/devops/toolset](http://newrelic.com/devops/toolset)