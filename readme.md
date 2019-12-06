# Data APIs as a service: Focusing on your core business
[Segment](http://segment.com) provides an easy way to collect data once about what users are doing and send the data to third party tools and warehouses. Segment does this by enabling businesses to collect first-party event data from their websites, mobile apps, and cloud tools like email and CRM, combine with offline data, then standardize and clean the data so it can be utilized in 200+ tools like marketing, analytics, attribution, and warehouses including Amazon Redshift.

[Segment * APIdays](https://events.segment.com/api-days-paris-2019) You know your core business depends on customer data. To help teams better understand customers, how many times do you use APIs to connect one tool to internal service to another tool? What other services have you built to support those connections? Join this workshop to build out your own APIs as a service for customer data.

Key takeaways include:

- Hooking up martech and analytics tools
- Collecting customer event and object data
- Scaling and supporting data pipelines


## Workshop Setup
Before following the exercises below, please download [Postman](https://www.getpostman.com/downloads/) and clone this repo for the Postman [environment](postman_info/postman_environment.json) & [request collection](postman_info/postman_collection.json).

```bash
git clone https://github.com/yabrira/apidays-workshop.git
```

If you would like to use cURL or do not have admin persissions to install applications, you can find the raw requests [here]().

## [Exercise 1](exercise1.md/) - Claiming your workspace and connecting a source
The focus of this [exercise](exercise1.md/) is to claim your workspace and to set up an HTTP source within the workspace. You will claim your workspace for yourself and we will walk through the process of configuring Segment to receive data an incoming HTTP request.

## [Exercise 2](exercise2.md/) - Ingesting data via HTTP and verifying your data
In this [exercise](exercise2.md/) we will pick up where we left off in the prior exercise by submitting a batch request into your HTTP source and verifying the accuracy of the data via our live debugger.

## [Exercise 3](exercise3.md/) - Configuring a downstream data consumer programmatically
In this final [exercise](exercise3.md/) use Segment's APIs to configure Google Analytics and Braze as downstream data consumers. 

## [Exercise 4 - Optional](exercise4.md/) - Providing a tracking plan to your API service environment
In this [exercise](exercise4.md/) we will add a data governance taxonomy to our event pipeline.
