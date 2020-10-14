# A SAP CAP Based Survey Application

The first step to develop the RQK application is the implementation of the
survey application for the end users. The applications is developed using the Javascript version of the
[SAP Cloud Application Programming Model (CAP)](https://cap.cloud.sap/docs/).

The development of the RQK application consists of the following steps:

* Initializing the CAP project
* Developing the database model
* Developing services based on the database model
* Developing the UI

## Prerequisites

Different development environments (cf. <https://cap.cloud.sap/docs/get-started/tools>) can be used to develop
applications in the SAP Cloud Application Programming Model. In this tutorial the SAP Business Application Studio
is used. Therefore, a new dev space for the SAP Business Application Studio needs to be created.
The new dev space should be of type **SAP Cloud Business Application**. In addition to the standard extensions
also the **Workflow Management** extension needs to be activated for this dev space.

Note that in the SAP Cloud Platform trail account there is a limitation regarding the dev spaces:
> You are allowed a maximum number of 2 dev spaces, and only 1 can be run at a time.

## Initializing the CAP project

Although the SAP Business Application Studio is used as a development environment, the
[CDS command line tools](https://cap.cloud.sap/docs/get-started/) are used to
initialize the CAP project. While the SAP Business Application Studio also provides
GUI based generators using the CDS command line tools is the most common approach. Being
used to the CDS command line tools also simplifies switching to different development environments later.

In order to use the CDS command line tools a terminal window is necessary. To open a new terminal window
in the SAP Business Application Studio right click on the empty projects pane and select
**Open in Terminal**.

![Open new terminal]("../img/rqk_cap_010.png)

This opens a new terminal window in the projects folder of the current dev space. In order to initialize a 
CAP project execute the following command in the terminal:

```bash
cds
```

This command prints out some general information regarding the CDS command line tools. Most importantly,
an overview of the available commands is given. Next execute 

```bash
cds help init
```

to get a list of the different available options for the ```cds init``` command. To initialize the
RQK application execute the following command.

```bash
cds i rqk
```

The result is an empty CAP project is generated inside the ```rqk``` folder. The empty projects consists of:

* the (empty) ```app```, ```db``` and ```srv``` folder
* the ```package.json``` file
* the ```README.MD``` file

## Developing the database model

* DB model
* model service
* CSV data
* in memory to real DB

## Developing services based on the database model

## Developing the UI

* add oData V2 proxy
* create admin list report
* https://blog.ui5cn.com/6-creating-custom-ui5-app-in-sap-capm-7-steps-to-get-started-with-sap-capm/
* https://www.youtube.com/watch?v=es0eAtAQPzk

## Navigation

* Next chapter: [RQK Workflow](../docs/rqk_workflow.md)
* Previous chapter: [RQK Overview](../docs/rqk_overview.md)