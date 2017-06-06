# IAAS Curriculum

In the following charter and the courses provided by the Institute of Architecture of Application Systems ([IAAS](http://www.iaas.uni-stuttgart.de/institut/mitarbeiter/indexE.php)) are discussed. The list of individual courses is presented [list of individual courses](#Spectrum) is discussed, and [several clusters of courses](#Clusters) emphasizing different foci are recommended.

These courses are motivated by the charter of IAAS that is sketched next.

## Charter of IAAS

The term *application system* is a piece of software supporting one or more core business activities of an enterprise. Typically, such a system 

* covers essential parts of the business activities of an enterprise,
* processes large amounts of persistent data, 
* enables a huge amount of users to operate concurrently with the system, and
* exchanges information with similar systems. 

An application system directly supports the business activities of an enterprise. Thus, it must satisfy strong requirements in terms of *non-functional properties* like availability, scalability, resiliency, and performance.

IAAS is concerned with the *architecture* of such enterprise systems, i.e. their underlying structure: What kind of building blocks and connections between them are needed to build such a system and guarantee its non-functional properties? In this context, IAAS is focussed on *middleware*, i.e. what kind of middleware is needed in the componentry of an architure of an application system, and how is such middleware used properly. Another concern are proper paradigms to *model* and specify application systems as well as their *compliance* with non-functional properties. 

In order to enable proper support of the various business activities of enterprises, IAAS investigates the role of *business processes* in application systems. Both, proper modelling of business processes as well as middleware needed to support them (so-called *workflow systems* or *process management systems*) as discussed. Business processes are considered as *programs in the large* and the composition of applications via business processes is investigated in terms of functionality as well as non-functional properties.

To support data exchange between application systems, IAAS is foucssing on *messaging systems* (message queuing, publish/subscribe) and *service technologies*. *Service-oriented computing* (SoC) and *Service-oriented Architecture* (SOA) are studied in general, specific service technology like *Web Services* and *REST*-based systems are investigated in particular. 

To support the operational requirements of applications systems like automatic provisioning and deployment as well as automatic management, the use of *Cloud Computing* as well as proper Cloud middleware and Cloud technologies are investigated. *Application topologies* and corresponding modeling languages are of particular interest. 

More and more, services are not only realized by software or human beings, but by also by sensors and actuators. Thus, IAAS is also concerned with the *Internet of Things* (IoT). 

*Transaction models* are discussed to ensure the robustness of application systems. In addition, the IAAS studies *optimization*-potentials of application systems in general, and of business processes in particular.

To support the transfer of research results into practice, IAAS has a special focus on patterns and *pattern lanugages*. Several pattern language have been proposed by IAAS. Furthermore, pattern languages themselves are a research focus of IAAS.

Finally, several application domains are of high interest at IAAS like *simulation technology*, *eScience*, *Digital Humanities*, and *manufacturing systems*.

This whole spectrum of topics is reflected in both, the research projects as well as the various courses of the IAAS. 

## <a name="Spectrum"></a> The Course Spectrum

The following figure shows the courses provided by IAAS. The layering of the courses from bottom to top is a first indicator of the sequence the courses should be taken - more details below.

![IAAS Courses](https://github.com/FrankLeymann/IAAS-Curriculum/blob/master/figures/Curriculum-Full.png "IAAS Courses") 

Dashed lines mean that these courses are not mandatory to any of the course clusters below. Nevertheless, they should be considered to complete the understanding of the overall subject area of IAAS. 

The following is a sketch of all courses from bottom (i.e. basic courses) to the top (i.e. more specialized courses).

### <a name="Modeling"></a> Modeling

*Conceptual data modeling* as well as *logical data modeling* is covered. Conceptual data modeling is introduced via of the *Entity-Relationship model*, logical data modeling by explaining the *relational mode*l of data. The latter includes *SQL* and *normalization theory*. *Transformations* from entity-relationship models as well as *XML schema* is discussed. Next, *UML* diagrams for modeling the static as well as the dynamic aspects of software systems is presented. The concept of *metamodeling* is discussed and *ontology modeling* is sketched. *Petri nets* and their analysis is covered, and *BPMN* for specifying process models is introduced. 

### <a name="GAAS"></a> Architecture of Enterprise Applications

The notion of an *architect* as well as *architecture* of application systems is discussed. Based on this, the *architectural diagrams* and architecture description languages (*ADLs*) are introduced, and different *architectural styles* are discussed. *Model-driven engineering* of software is motivated. *Non-functional properties* are introduced and related to architectural modeling. *Transactions* are covered by discussing the ACID paradigm, concurrency control, and advanced transaction models. Synchonous as well as asynchronous communication is discussed along with *RPC* middleware and *message queuing* middleware. The concept of *APIs* is introduced. Based on the before, *TP monitors* as well as *application servers* are presented. A detailed discussion of *high availability*, *scalability*, *stability*, and *consistency* follows. *Pattern languages* are introduced, and first sketch of *patterns of enterprise applications* as well *cloud computing patterns* is given. 

### <a name="LCM"></a> Loose Coupling and Message-Based Applications

The notion of *enterprise application* is introduced. Based on this the need for *loose coupling* is derived and its realization via *reliable messaging* sketched. *Message-oriented middleware* (MOM)and a sample *MOM architecture* is discussed in detail, and *JMS* as a supporting standard API is presented. Next, *basic integration styles* are outlined and a survey of the *enterprise integration pattern* language is given. This language is then discussed in depth: *messaging*, messaging *endpoints*, message *channels*, message *construction*, message *routing*, message *transformation*, message *management*. The concept of a *message bus* is sketched.
 
### <a name="SoC"></a> Service Computing

The Web is presented as a *platfrom for applications*, and an overview on related trends like the Semantic Web, Cloud Computing, or Autonomic Computing is given. The notion of a *service* and *service computing* is introduced. Some Web-based user interface technologies are briefly sketched. *HTTP* is discussed in detail. Based on that, *REST* is introduced and a design method for REST-based interfaces is presented. An overview on e-*mail* related protocols is given. *SOAP*, *WSDL* and *Policy* are introduced extensively, service *discovery* is touched. *Axis* is briefly sketched. *Agreement protocols* and *coordination* are discussed in depth. Finally, the overall architecture of a *service bus* is portrayed, ongoing discussions like *microservices*, *big vs small Web Services* are commented on. 

### <a name="BPM"></a> Business Process Managment

An overview on the *evolution* of business process management technology begins the lecture. The *business process management lifecycle* is presented and *business process (re-)engineering* is discussed in depth. A quick introduction into *Petri nets* is given to understand the execution semantics of BPMN, and *BPMN* is discussed extensively. Next, basic concepts and architectural aspects of *workflow management systems* (WfMS) are introduced. A *graph-based metamodel* for process models is discussed and used to formally define key concepts like *control flow*, *data flow* and *dead-path elimination*. A discussion of *transactional workflows* follows. Finally, *BPEL* is presented in detail. 

### <a name="aBPM"></a> Advanced Business Process Managment

The concept of *subprocesses* and corresponding *coordination* technology is introduced. *Human Tasks* and *human oriented processes* as well as corresponding middleware is discussed in detail. Advanced modeling paradigms like *pi-calculus* as well as *workflow patterns* are presented. Requirements and problems of *adaptive workflows* are discussed, and an overview on *case handling* including *CMMN* is given. The role of business process technology in *outsourcing* and especially *choreographies* are introducewd. *Process compliance* is covered, and the role of *process mining* including its algorithmic aspects is revealed. 

### <a name="Cloud"></a> Cloud Computing 

A description of *Cloud Service- and Deployment Models* begins the lecture. Next, *virtualization* as well as *containerization* is presented. The realization of *scalability* as well as *elasticity* in cloud environments is revealed. *Architectural aspects* of cloud applications, i.e. *cloud native* and *cloud immigrant* is discussed. *Provisioning* paradigms and technology is presented in detail. Several cloud offerings, like *Amazon Web Services* or *Cloud Foundry* are sketched. The *cloud computing pattern language* is presented, the individual patterns of which are intervowen with the presentation of the concepts and technologies of the lecture.  

### <a name="pract"></a> Practical Courses

The practical courses are *lab courses* with hands-on concrete technology. *Programming assignments* are given that have to be worked on and solved by the students. The *Cloud* practical course is focussing on cloud technology, the *REST, SOA, BPM* practical course on exactly those. 

### <a name="ITS"></a> IT Strategy

(The course is given in German.) After clarifying the term "strategy", *enterprise strategy* and *IT strategy* are introduced. A corresponding *processing model* for developing such strategies is presented and explained based on concrete *use cases*. The relation to *ITIL* and *CoBIT* is revealed. Individual processes for *organization development*, *IT sourcing*, *architecture management*, *quality management*, *risk management*, *IT development plan* are discussed in detail. Corresponding *tools* will be presented. A sketch on *IT portfolio management* and *IT metrics* complete the lecture. 

### <a name="SM"></a> Systems Management

This course is given as a collection of presentations by industry practitioners mostly. The actual content of the lecture is determined by hot topics in the industry. The presentations are embraced by two lectures at the beginnig and the end that position the individual presentations to the overall subject. 

### <a name="Proj"></a> Hands-On Projects

Hands-on projects are performed in teams and are oriented on actual research projects of the institute. Thus, state-of-the-art technology will be used to contribute to solutions of concrete research problems. Participant in such projects work at the forefront of technology. 

## <a name="Clusters"></a> Course Clusters





![IAAS Courses](https://github.com/FrankLeymann/IAAS-Curriculum/blob/master/figures/Integration-Cluster.png) 



![IAAS Courses](https://github.com/FrankLeymann/IAAS-Curriculum/blob/master/figures/Cloud-Cluster.png) 



![IAAS Courses](https://github.com/FrankLeymann/IAAS-Curriculum/blob/master/figures/BPM-Cluster.png) 



![IAAS Courses](https://github.com/FrankLeymann/IAAS-Curriculum/blob/master/figures/System-Architect-Cluster.png) 





![IAAS Courses](https://github.com/FrankLeymann/IAAS-Curriculum/blob/master/figures/Enterprise-Architect-Cluster.png) 


