![](misc/img/home_slide.svg)

# Workshop: Getting started with Segment programmatically

Many collection APIs exist out there in the wild. Some focus on real-time and others queue messages and release them in a cron-job style fashion. The power of APIs is almost endless, but the ease of use comes with one drawback: __Every tool has an API!__ The overall expansion of technology and software that consumes customer data in one way or another has put a tremendous strain on developers and marketers. The need to instrument “n” amount of APIs with all their nuances and intricacies is causing bottlenecks and technical debt. Questions like, “Where are the docs for this?” or statements such as, “Let’s check what StackOverflow says about this,” are becoming more present, and a developer might need to “know” 5-25 different APIs besides the work they are already doing. Segment aims to overcome this by providing an API first design to the customer data problem and turning your collection of APIs into a service, ultimately allowing you to focus on your core business.

[Segment](http://segment.com) provides companies an easy way to collect, clean, and connect their first-party data to the applications they need to run their businesses. Segment does this by enabling businesses to collect first-party event data from their websites, mobile apps, and cloud tools like email and CRM, combine with offline data, then standardize and clean the data so it can be utilized in 300+ tools like marketing, analytics, attribution, and warehouses including Amazon Redshift.

[Segment * Data Innovation Summit](https://events.segment.com/api-days-paris-2019) You know your core business depends on customer data. To help teams better understand customers, how many times do you use APIs to connect one tool to internal service to another tool? What other services have you built to support those connections? Join this workshop to build out your own customer data infrastructure.

Key takeaways include:

- Collecting customer event and object data
- Hooking up martech and analytics tools
- Scaling and supporting data pipelines


## Workshop Setup
Following along will require the following:

- A Segment workspace 
- A Google Analytics account
- The ability to make HTTP requests


## [Preparation](preparation.md/) - Creating your workspace and connecting a source
The focus of this [exercise](preparation.md/) is to prepare your workspace for exercise 1 & 2. You will claim your workspace for yourself and we will walk through the process of configuring Segment to receive data via an incoming HTTP request.

## [Exercise 1](exercise1.md/) - Ingesting data via HTTP and verifying your data
In this [exercise](exercise1.md/) we will pick up where we left off in the prior exercise by submitting requests into your HTTP source and verifying the accuracy of the data via our live debugger.

## [Exercise 2](exercise2.md/) - Configuring a downstream data consumer programmatically
In this final [exercise](exercise2.md/) we'll use Segment's APIs to configure Google Analytics and Braze as downstream data consumers. 

P.S. If you are doing this workshop outside of the webinar, please set up your own workspace and follow the steps from [Preparation](preparation.md/) Part 2.