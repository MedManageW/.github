# MedMangeW

Authors: [Xiaxi Shen](https://github.com/xshen053), [Shao-Jung(James) Kan](https://github.com/hjameskan), [Yenyen Liao](https://github.com/yenyenn19), [Eric Chang](https://github.com/echang1116), [Ivan Zenkovitch](https://github.com/IvanZenk), [Zichao Chen](https://github.com/zcchen21)

## Project Background

The Digital Medication Management project is sponsored by Novo Nordisk. Alzheimer’s Disease patients often experience memory loss, confusion, and comorbidities. With multiple diseases occurring simultaneously, they often need to take multiple medications at a time, also known as polypharmacy. Polypharmacy can possibly cause contraindications of medications, as multiple medicines are being taken at once and they could possibly contradict each other and result in side effects. These contraindications can be hard to catch when prescribing the medications, therefore could potentially pose great danger to the health of the patients. In addition, people with Alzheimer’s Disease experience memory loss and often forget to take the medications on time. The objective of this project is to deliver a solution to deal with the issue of polypharmacy for patients with Alzheimer’s disease, and remind them to take the medications on time.

## Project Description

We are delivering a solution for Alzheimer's patients;

The solution has a software component, which is a mobile app for patients, doctors, and caregivers to keep track of the medications that the patients are currently taking and detect any medical contraindications, as well as a hardware component, which dispenses the medications at the right time and reminds the patients to take the medications.

## Our Tech Stack

### Software Team

[Xiaxi Shen](https://github.com/xshen053), [Shao-Jung(James) Kan](https://github.com/hjameskan), [Yenyen Liao](https://github.com/yenyenn19)

- [React Native](https://reactnative.dev/) - We will leverage the power of React Native, an open-source framework developed by Facebook, to build our mobile application. With React Native, we can write our app's code in JavaScript and create native-like mobile experiences for both iOS and Android platforms. Its declarative approach and extensive UI component library make it efficient and intuitive to develop highly dynamic and interactive user interfaces. Additionally, React Native's performance optimizations ensure that our app runs smoothly and efficiently, providing a seamless user experience.

- [Redux](https://redux.js.org/) - Redux is a predictable state container for JavaScript apps. It is often used with libraries like React or Angular for building user interfaces. The main idea of Redux is that the entire state of an application is stored in a single central place called a "store". Actions trigger changes in this store, and the changes are made with pure functions called "reducers". This pattern can make it easier to reason about how state changes over time and to manage complex state that is shared among many components.

- [PostgreSQL](https://www.postgresql.org/) - PostgreSQL is an advanced, open-source relational database system. It supports both SQL (relational) and JSON (non-relational) querying. PostgreSQL is highly extensible and allows for custom functions; it's highly scalable both in the sheer quantity of data it can manage and in the number of concurrent users it can accommodate. It has robust support for distributed and parallel computing.

- [AWS: RDS](https://aws.amazon.com/rds/) - RDS is a web service provided by Amazon Web Services (AWS) that makes it easier to set up, operate, and scale a relational database in the cloud. It supports several types of databases including PostgreSQL, MySQL, MariaDB, Oracle, and Microsoft SQL Server. It takes care of routine database tasks such as backup and restore, patch management, and replication.

- [AWS: S3](https://aws.amazon.com/s3/) - S3 is an object storage service offered by AWS. It's designed to store and retrieve any amount of data from anywhere on the web. It provides scalability, high availability, and low latency with strong consistency. It's commonly used for backup and restore, archiving, content distribution, and data lakes for analytics.

- [AWS: Route53](https://aws.amazon.com/route53/) - Route53 is a scalable and highly available Domain Name System (DNS) web service provided by AWS. It is designed to give developers and businesses a reliable and cost-effective way to route end users to Internet applications by translating domain names into the numeric IP addresses that computers use to connect to each other. Route53 also provides domain registration services, where you can register new domain names.

- [AWS: CodePipeline](https://aws.amazon.com/codepipeline/) - CodePipeline is a fully managed continuous integration and continuous deployment (CI/CD) service from AWS. It helps automate the build, test, and deploy phases of your release process every time there is a code change, based on the release model you define.

- [AWS: Elastic BeanStalk](https://aws.amazon.com/elasticbeanstalk/) - Elastic Beanstalk: Elastic Beanstalk is a Platform as a Service (PaaS) provided by AWS. It allows developers to deploy and manage applications without having to understand the underlying infrastructure, as it automatically handles the capacity provisioning, load balancing, scaling, and application health monitoring. It supports several major languages, web servers, and databases.

- [Express](https://expressjs.com/) -

- [Sequelize](https://sequelize.org/) -

- [JavaScript](https://code.visualstudio.com/) - We use JS for frontend and backend development

- [Visual Studio](https://cmake.org/) - We will use Visual Studio as an ide to develop the software.

- [Git](https://git-scm.com/) - We will use Git as the version control tool to coordinate work, keep track of changes in our code, and keep our project up to date.

### Hardware Team

[Eric Chang](https://github.com/echang1116), [Ivan Zenkovitch](https://github.com/IvanZenk), [Zichao Chen](https://github.com/zcchen21)

- [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) - We used JavaScript for backend development of the dispenser.

- [Node.js](https://nodejs.org/) - We used Node.js for the server of our dispenser, which is a light-weight and efficient environment that uses JavaScript for building server-side applications

- [Express](https://expressjs.com/) - The Express framework is used to simplify the process of building the server and APIs, specifically used for defining routes to handle HTTP requests and utilizing middleware to parse request bodies and error handling.

- [Axios](https://axios-http.com/) - We used Axios to send HTTP requests from the dispenser to the mobile app for communication purpose

- [PM2](https://pm2.keymetrics.io/) - PM2 is used to manage and run the servers of the dispenser in the background, and handles automatic reboot when the server crashed

- [Ngrok](https://ngrok.com/) - ngrok is used to forward the requests of the local server to a public URL that can be reached from anywhere in the world

- [Arduino Mega](https://store.arduino.cc/arduino-mega-2560-rev3) - The Arduino Mega board is the microcontroller that we use to communicate with the AML-S905X-CC and to control the connected peripherals. The Arduino Mega receives  and sends commands on a serial port connected to the AML-S905X-CC. The Arduino Mega houses 54 digital pins, many of which are used to control the stepper motors which drive the dispenser.

- [C++](https://en.cppreference.com/w/) - The code for the Arduino Mega is written in a subset of C++, known as the Arduino Language. This language allows for low-level access to hardware and high performance, making it suitable for programming microcontrollers. We make use of the default Arduino library, as well as the Arduino Stepper Motor library.

- [AML-S905X-CC](https://www.96boards.org/product/tinker-board-s/) - The AML-S905X-CC (Le Potato) is a single board computer that we use to host the dispenser server. 

- [Ubuntu Server](https://ubuntu.com/server) - The Ubuntu server provides a Linux environment to run all of the applications and servers of the dispenser

- [28BYJ-48 Motor](https://www.adafruit.com/product/858) - The 28BYJ-48 motor and ULN2003 stepper motor drivers are used to control each compartment of the physical dispenser. This stepper motor is sufficiently accurate enough to consistently dispense medication, and it is easily controlled with built in Arduino libraries. 

<!-- 
- The input of our project would be []
- The output of our project would be [] -->

## Overall Design

![img3](https://github.com/MedManageW/.github/blob/main/resources/OverallDesign.png)

<!-- ## Example picture and description

## Installation/Usage

## Testing -->

<!-- ![img3](https://github.com/MedManageW/.github/blob/main/resources/OverallDesign.png)
![img1](https://github.com/MedManageW/.github/blob/main/resources/AppScreen1.png)
![img2](https://github.com/MedManageW/.github/blob/main/resources/AppScreen2.png)
![img4](https://github.com/MedManageW/.github/blob/main/resources/hardware1.png)
![img5](https://github.com/MedManageW/.github/blob/main/resources/hardware2.png)
![img6](https://github.com/MedManageW/.github/blob/main/resources/hardware3.jpg) -->
