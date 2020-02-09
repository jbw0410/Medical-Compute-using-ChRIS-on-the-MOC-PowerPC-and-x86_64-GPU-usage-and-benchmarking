# Medical-Compute-using-ChRIS-on-the-MOC-PowerPC-and-x86_64-GPU-usage-and-benchmarking

## 0.   Contributors:

**Mentor**: Rudolph Pienaar (rudolphpienaar)

**Group Members**:

Elizabeth Slade (https://github.com/emslade23)

Shineun Yoon (https://github.com/ShineunYoon)

Bowen Jia (https://github.com/jbw0410)

Haoyang Wang (https://github.com/PupilTong)

Kefan Zhang (https://github.com/h4x0rMadness)

**ChRIS Introduction**:

Red Hat "Creating ChRIS": https://www.redhat.com/en/creating-chris

Boston University Red Hat Collaboratory of ChRIS : https://www.bu.edu/rhcollab/projects/radiology/

## 1.   Vision and Goals Of The Project:

The overall vision of this project is to develop a plugin based on ChRIS platform so that users like developers or administritors are able to do benchmarking between different architectures like x86 and PowerPC.

For the following sprints of this project, we are going to get familiar with Mass Open Cloud, ChRIS platform, ChRIS plugins and benchmarking methods in order to integrate all the components and implement the benchmarking plugin on ChRIS platform for the future use.


### High-level goals include:


- Improve the functions of our benchmarking ChRIS plugin 

- Use the real work environment to further improve the ChRIS plugin to better benchmark


## 2. Users/Personas Of The Project:

User Persona Examples:
- ChRIS developers and ChRIS administrators who want to understand how the ChRIS platform runs on different network topologies. 
- Researchers/Developers who want to benchmark and compare the efficiency of different network topologies for their experiments.




Non-target users are:
- Clinicians/Technicians who don’t use MOC, ChRIS.
- Clinicians/Technicians want software that is easy to use, that is informative when helping them make a diagnosis and that is able to compute results quickly so that clinicians can maximize their time with their patients and make more informed decisions. 
- Researchers/Developers who want an open-source environment with accessible documentation, efficient computational resources, and useful plug-ins so that they can conduct efficient experiments on medical data in the cloud.
- Healthcare organizations who want their doctors to make data driven diagnoses about patients so that the organization increases their credibility and reliability. 
- Healthcare organizations who want to be on the cutting edge of medical computing technology and analysis so that they can provide the best healthcare for their patients.


** **

## 3.   Scope and Features Of The Project:

We will focus on one plug-in which provides a series of tools and test functions to test the performance of the system. The test functions may cover from a simple matrix multiplying to a huge neural network training, to represent the real workloads that may be deployed on the system. For example, if the real functions move data between main memory and GPU memory frequently, our functions are supposed to show this feature.


However, we are not focusing on building a precious and complex machine learning model or data processing method. All test functions will run fast, estimating time may spend on running real computing tasks in an acceptable time span, like several minutes. Therefore, they should emulate the real ChRIS workloads as light as possible. Since there is no reason to run a benchmark for 8 hours rather than run a real task for 8 hours to ESTIMATE the performance.

At last, this plugin will produce comparable results that allow users to compare the performance of different platforms in an elegant and easy method.

## 4. Solution Concept

### Global Architectural Structure Of the Project:

This section provides a high-level architecture or a conceptual diagram showing the scope of the solution. If wireframes or visuals have already been done, this section could also be used to show how the intended solution will look. This section also provides a walkthrough explanation of the architectural structure.

### Design Implications and Discussion:

The goal for the ChRIS platform is to provide a containerized application that is made up of many plugins which run specific functions on inputs. The scope for our portion of the project is to develop one plugin that runs a function to benchmark performance between different architectures. The reason for this design decision is to make the plugin easy to use and integrate with a clinician or technicians workflow. 

The implications for our global architecture design are to allow for clinicians using ChRIS to benchmark different architectures to find the archtecture that works the fastest for given medical computations.

## 5. Acceptance criteria

Correctly developed a runnable ChRIS plugin that to some extent presents the performance difference between different platform architectures.
The minimal product presents the benchmark differences between x86 and PowerPC.


## 6.  Release Planning:

The release planning section describes how the project will deliver incremental sets of features and functions in a series of releases to completion. Identification of user stories associated with iterations that will ease/guide sprint planning sessions is encouraged. Higher-level details for the first iteration is expected.

### Sprint 1: February 12th, 2020

Get familiar with the ChRIS platform, either from web-app/ terminal operations.  
	
Set up environments for future development. (Linux/ docker)  

Research on how to use MOC(Mass Open Cloud)

Get the NIST dataset and research on training the ML model. 


### Sprint 2: February 26, 2020

Build out the Machine learning/ neural network application

Be able to run operations on the MOC computers

Be able to run plugins from the local ChRIS instance

### Sprint 3: March 7, 2020

Be able to run a pre-existent plugin via ChRIS on the MOC GPUs.

Develop benchmarking metrics to analyze plugin processes. 

Upload our Machine learning/ neural network application plugin to a ChRIS instance using containerization.

### Sprint 4: March 20, 2020

Integrate our plugin into the app store.

Get more granular with benchmarking metrics




** **

## General comments


