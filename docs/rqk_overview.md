# The High-Level Architecture of the Red Qualtrics Killer

In the next part of this tutorial an extension to the existing backend application is developed.
The goal of this part is to show the possibility of extending existing ERP systems using the 
SAP Cloud Platform.

The RQK application consists of the following SAP Cloud Platform components:

* A SAP Fiori application
* A database and services build using the [SAP Cloud Platform Programming Model](https://cap.cloud.sap/docs/)
* A workflow build using different SAP Cloud Platform services.

The following process is implemented using these components:

1. Once an order is set to the status *complete* in the POM a workflow instance in the SAP Cloud Platform Workflow
service is started.
1. This workflow creates an open review in the RQK database
1. The workflow sends an email to the contact person of the order asking for a review of the order process.
1. One the review is completed business rules modeled using the SAP Cloud Platform Business Rules service are used
to determine the next process steps. If a bad review is provided a task to contact the customer is created in the
workflow inbox of the user.

## Navigation

* Next chapter: [RQK Survey Application](../docs/rqk_survey.md)
* Previous chapter: [Extending the Sales Order BOPF Object](../docs/order_monitor_bopf.md)