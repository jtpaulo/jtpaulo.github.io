---
layout: archive
title: ""
permalink: /portfolio/
author_profile: true
---

{% include base_path %}

# Projects

### [BigHPC: A Management Framework for Consolidated Big Data and HPC (POCI-01-0247-FEDER-045924)]()

**2020-Current**: The BigHPC  project will provide a novel management framework, for Big Data and parallel computing workloads, that can be seamlessly integrated with existing HPC infrastructures and software stacks. The project will research, develop and integrate new monitoring, virtualization, and storage management components that can cope with the infrastructural scale and heterogeneity, as well as, the different workload requirements, while ensuring the best performance and resource usage for both applications and infrastructures. I am the coordinator of INESC TEC's activities in the project. The project includes the following partners: Wavecom (coordinator), INESC TEC, LIP, MACC, TACC, UT Austin

### [PAStor: Programmable and Adaptable Storage for AI-oriented HPC Ecosystems (PT-UTAustin Exploratory Project)](http://bighpc.inesctec.pt)

**2020-Current**: The PAstor project aims at providing a novel Software-Defined Storage (SDS) solution for HPC that can efficiently handle I/O flows from multiple AI workloads by automatically adjusting storage configurations and resources to meet applications dynamic requirements. The project will provide the first building blocks towards a novel storage architecture tailored for AI applications deployed at exascale computing infrastructures. I am one of the coordinators of the project. The project includes the following partners: INESC TEC (coordinator), TACC (coordinator)MACC, Hood College

### [Efficient and Secure Data Management for HPC and Cloud Computing (CENTRA project)](http://www.globalcentra.org/projects/#prv)

**2018-Current**: The "Efficient and Secure Data Management for HPC and Cloud Computing" project aims at researching novel data management solutions for Cloud and HPC distributed environments. These solutions must be efficient, secure, and practical by: 1) alleviating any storage or processing performance bottlenecks identified for data-centric applications deployed on HPC and Cloud services; 2) following a privacy-by-design approach when storing and processing sensitive data on third-party infrastructures; and 3) re-using stable and industry-adopted storage systems, databases and analytical platforms. I am currently the coordinator of this project, which is being done in collaboration with the KISTI and AIST research centers (South Korea and Japan). It also includes external collaborations with researchers from TACC and UT Austin.

### [IBM Research Haifa Joint Study Agreement]()

**2018-2020**: IBM Research Haifa and INESC TEC participate in a joint study in which the parties will do research on novel benchmarking solutions for storage systems with deduplication and compression capabilities, and on novel secure and privacy-preserving storage paradigms. I am currently the coordinator of this project on behalf of HASLab.

### [SafeCloud (H2020-DS-2014-1/653884)](http://www.safecloud-project.eu/)

**2015-2018**: Cloud infrastructures, despite all their advantages and importance to the competitiveness of modern economies, raise fundamental questions related to the privacy, integrity, and security of offsite data storage and processing tasks. There are major privacy and security concerns about data located in the cloud, especially when data is physically located, processed, or must transit outside the legal jurisdiction of its rightful owner. These questions are currently not answered satisfactorily by existing technologies. SafeCloud will re-architect cloud infrastructures to ensure secure and private data transmission, storage, and processing. My work on this project led to the conception and development of privacy-preserving databases and filesystems.

### [A Coherent and Rich PaaS with a Common Programming Model (FP7-ICT-2013-10/ 611068)](http://coherentpaas.eu/)

**2015-2016**: CoherentPaaS combines in an integrated platform SQL (OLTP, in-memory analytics, OLAP), NoSQL (key-value, document-oriented and graph databases) and CEP/data streaming. In this platform applications can start global transactions and update any combination of data stores with full transactional semantics. Applications can also make queries across data stores combining the simplicity of SQL with the power of the underlying native query languages. My work involved the conception of a scalable transactional logging mechanism for large-scale distributed databases

### [RED: Resilient Databases (PDTC/EIAEIA/109044/2008)](http://red.lsd.di.uminho.pt/)

**2010-2012**: It might look simple at first sight to extend the shared-nothing protocol to cope with shared storage: If all replicas perform exactly the same write operations, database state would be identical and thus could be shared. Unfortunately, internal non-determinism means that different physical images are produced regardless of logical consistency, leading to corruption. Moreover, such simple approach would not preserve the logical independence of replicas and rule out tolerating Byzantine faults. The ReD approach is to combine the replication protocol with a specialized copy-on-write volume management system, that holds transient logically independent partial copies, thus masking internal server non-determinism and isolating multiple logical replicas for resilience. My work was focused on database replication, shared storage cluster and storage virtualization. More specifically, the shared-storage cluster approach using mySQL was ported to a virtualized environment that uses XEN.


# Software


### [SafeFS](https://github.com/safecloud-project/safefs)

SafeFS is a software-defined file system based on a modular architecture featuring stackable layers that can be combined to construct a secure distributed file system. SafeFS allows users to specialize their data store to their specific needs by choosing the combination of layers that provide the best safety and performance tradeoffs. The prototype is implemented in user space using FUSE The provided layers include mechanisms based on encryption, replication, and coding.


### [DEDISBench](https://github.com/jtpaulo/dedisbench)

DEDISbench is an open source micro I/O benchmark suitable for evaluating deduplication systems by generating blocks with a realistic content distribution. The benchmark also allows running tests with different load intensities and introduces a novel hotspot access pattern for I/O requests.


### [DEDIS]()

DEDIS is a novel open source distributed post-processing deduplication system. Its main contribution is a novel optimistic asynchronous mechanism for eliminating duplicated data among virtual machines deployed on several remote hosts. This mechanism along with other optimizations allows achieving nearly native disk I/O throughput for virtual machines even when deduplication is being performed in the background. Additionally, DEDIS is fully distributed, allowing the system to scale, and is resilient to server crashes.
