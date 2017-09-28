# Distributed Enabling Platforms

* Teacher: [Nicola Tonellotto](http://pomino.isti.cnr.it/~khast/)
* CFU: 6
* Period: First semester
* Language: English
* Lectures schedule: Monday 16--18 (L1) and Friday 9--11 (A1).
* Backup lectures: Thursday 16--18 (CNR, Room C32)
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

|Date|Lecture|Topics|Slides|
|:--:|:-----:|------|:----:|
|18/09| 16 - 18 | Introduction, Clouds and Datacenter. | [Slides (PDF)](./slides/introduction.pdf)|
|22/09| 9 - 11 | MapReduce: challenges, difficulties, design ideas. Programmin model: mappers, reducers, shuffle and sort. Word count example. | [Slides (PDF)](./slides/mr1.pdf)|
|25/09| 16 - 18 | Hadoop: basic classes (Mapper and Reducer), jobs, basic and complex data types, Word Count implementation in Hadoop. Input and Output in MapReduce. | [Slides (PDF)](./slides/mr2.pdf)|
|29/09| 9 - 11 | Hadoop execution modes, installation, programming, execution. HDFS command-line interface. | [Notes (MD)](./notes/hadoop-installation.md)|
|02/10| 16 - 18 | LECTURE CANCELLED.

## Tentative Topics
The following list of topics is subject to change.

| Topic | Description | References |
|--------|-------------|------------|
|Datacenters & Cloud | Big data and large scale problems. The Cloud paradigm and the datacenter as a computer.| [BCH] Chapters 1 and 4. |
| MapReduce Programming Model | Basics, partitioners, combiners, design patterns, I/O, physical execution, data storage | [MMD] Chapter 2, [LIN] Chapters 1.2, 2,  3.1, 3.2, 3.3, 5.1 and 5.2.|
| Programming in Hadoop| Installation and configuration, I/O, interfaces, types and formats. | [TW] |
| Algorithms in MapReduce: | Real-world problems solved with MapReduce: PageRank, Inverted Indexing, Near Duplicate Detection | [LIN] Chapters 4.1, 4.2, 4.3, 4.4 and 5.3. [MMD] Chapters 3.1, 3.2, 3.3. and 3.4. |
| Data models, representation and storage| Relational, document and graph models, SS Tables, LSM trees, format and encoding of data (Thrift, Avro, Protocol buffers) | [DDIA], Chapters 3 and 4.|
| Data management and replication | Leaders and followers, single leader and multi leader replication, leaderless replication, consistent hashing | [DDIA] Chapter 5.|
| Data Consistency & Consensus | Consistency Models, Eventual Consistency, Consensus, FLP and CAP Theorems| Slides |
| Time in distributed System | Events, scalar clocks, vector clocks, global state | [TIME] |
| Web Serch Engine Infrastructure| Crawling, Indexing, Query Processing| [WSE]|

## References

* The Datacenter as a Computer, 2nd edition, L. A. Barroso, J. Clidaras, U. Hölzle, Morgan & Claypool Publishers, 2013\. ([Amazon](https://www.amazon.com/Datacenter-Computer-Introduction-Warehouse-Scale-Architecture/dp/1627050094)) [BCH]
* Mining of Massive Datasets, J. Leskovec, A. Rajaraman, J. Ullman, Cambridge University Press, 2014\. ([link](http://www.mmds.org)) [MMD]
* Data-Intensive Text Processing with MapReduce, J. Lin, C. Dyers, Morgan & Claypool Publishers, 2010\. ([link](https://lintool.github.io/MapReduceAlgorithms/MapReduce-book-final.pdf)) [LIN]
* Hadoop -- The Definitive Guide, 4th edition, T. White, O'Reilly, 2015\. ([Amazon](https://www.amazon.com/Hadoop-Definitive-Storage-Analysis-Internet/dp/1491901632)) [TW]
* Designing Data-Intensive Applications: The Big Ideas Behind Reliable, Scalable, and Maintainable Systems, D. Kleppmann, O'Reilly, 2017\. ([Amazon](https://www.amazon.com/Designing-Data-Intensive-Applications-Reliable-Maintainable/dp/1449373321)) [DDIA]
* Scalability Challenges in Web Search Engines, B. B. Cambazoglu R. Baeza-Yates, Morgan & Claypool Publishers, 2016\. ([Amazon](https://www.amazon.com/Scalability-Challenges-Synthesis-Information-Retrieval/dp/1627058125)) [WSE]
* Lecture notes on logical time and synchronization, University of New South Wales ([link](http://www.cse.unsw.edu.au/~cs9243/15s1/lectures/synch-notes.pdf)) [TIME]
