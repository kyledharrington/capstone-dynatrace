# So you want to be a Dynatrace Sales Engineer

Thank you for your interest in being a part of the Sales Engineering team at Dynatrace. As next steps we will ask you to setup and demo an environment of your choosing to the Sales Engineering team instrumented by the Dynatrace platform. The goal of this demo is to highlight your technical aptitude by demonstrating the core concepts and feature functionality of the Dynatrace platform and your ability to present value of the Dynatrace platform to prospects across multiple business units in a single presentation.

See below for further instructions and expectations of this demo and reach out to your hiring manager or kyle.harrington@dynatrace.com with any questions.

1. Sign up for a free Dynatrace SaaS trial 
    - https://www.dynatrace.com/trial/

1. Deploy OneAgent to your environment
    - [Linux](https://docs.dynatrace.com/docs/setup-and-configuration/dynatrace-oneagent/installation-and-operation/linux/installation/install-oneagent-on-linux)
    - [Windows](https://docs.dynatrace.com/docs/setup-and-configuration/dynatrace-oneagent/installation-and-operation/windows/installation/install-oneagent-on-windows)
    - [Kubernetes](https://docs.dynatrace.com/docs/setup-and-configuration/setup-on-k8s/installation/classic-full-stack)

1. Deploy a Web Application

    Dynatrace has a general purpose application you can leverage for this demo, Easy Travel. Easy travel consists of an nginx front end, java backend and sql db. 

    - [Easy Travel - Standalone](https://community.dynatrace.com/t5/Getting-started/easyTravel-Documentation-and-Download/td-p/181271)
    - [Easy Travel - Docker](https://github.com/Dynatrace/easyTravel-Docker)

    

1. Alternatively, you can choose to use any other web frontend you have already worked with or built for this demo

    Requirements of the test application if not using Easy Travel
    - Front End browser web component 
    - http service level calls 
    - Backend Database
    - Ideally, the application will be capable of generating errors/ crashes/ outages
    - Check [Dynatrace's list of supported technologies](https://docs.dynatrace.com/docs/setup-and-configuration/technology-support) for technology compatibility

   Other public web applications:
    - [Kona Kart](https://github.com/BraydenNeale/dynatrace_konakart_docker)
    - [Google's Hipster Shop](https://github.com/lightstep/hipster-shop)
    - [Google's Online Boutique](https://github.com/GoogleCloudPlatform/microservices-demo)

1. External integrations and extensions

    Setup of the below additional Dynatrace integrations and extensions to setup and demo in your environment. These are intended to be challenging and highlight how your previous experience will translate to Dynatrace's Sales Engineering team. The below are tiered in challenge level of time and technical ability to implement. Dynatrace documentation links are included. Please note, these are only examples. 

    Required Configurations for your Demo:
        
    - [Configure a problem notification systems outbound from Dynatrace, that is NOT email](https://docs.dynatrace.com/docs/observe-and-explore/notifications-and-alerting/problem-notifications)
    - [Create a Management Zone](https://docs.dynatrace.com/docs/manage/access-control/management-zones/set-up-management-zones)
    - [Add a Synthetic check to your web application](https://docs.dynatrace.com/docs/platform-modules/digital-experience/synthetic-monitoring)
    - [Setup Tagging Rules for your environment](https://docs.dynatrace.com/docs/manage/tags-and-metadata/setup/how-to-define-tags)
    - [Enable Session Replay Capture](https://docs.dynatrace.com/docs/platform-modules/digital-experience/session-replay/enable-session-replay-web)
 
    Additional Optional Integrations (strongly encourged that some of these are present)

    Feel free to review the Dynatrace [Getting started with Dynatrace](https://docs.dynatrace.com/docs/get-started) and [Product News](https://www.dynatrace.com/news/blog/) pages and come up with your own integration ideas for you demo. Make sure you call these out during your demo if you set them up 

    - [Configure Conversion Goals](https://docs.dynatrace.com/docs/platform-modules/digital-experience/web-applications/analyze-and-use/define-conversion-goals)
    - [Define Session Properties](https://docs.dynatrace.com/docs/platform-modules/digital-experience/web-applications/additional-configuration/define-user-action-and-session-properties)
    - [Add any metric data point(s) to your environment using Metric Ingestion](https://docs.dynatrace.com/docs/extend-dynatrace/extend-metrics/ingestion-methods/oneagent-metric-api)
    - [Instrument a Python application with OneAgent](https://github.com/dynatrace-oss/OneAgent-SDK-Python-AutoInstrumentation)
    - [Add a Synthetic check to you web app via a *Private* active gate](https://docs.dynatrace.com/docs/platform-modules/digital-experience/synthetic-monitoring/private-synthetic-locations/create-a-private-synthetic-location)
    - [Use the Events API to add Event data to an entity](https://docs.dynatrace.com/docs/dynatrace-api/environment-api/events-v2/post-event)
    - [Integrate Dynatrace with a Cloud Account](https://docs.dynatrace.com/docs/platform-modules/infrastructure-monitoring/cloud-platform-monitoring)
    - [Integrate your environment with LoadRunner, JMeter or Neotys](https://docs.dynatrace.com/docs/shortlink/load-testing-process#available-integrations)
    - [Leverage the Dynatrace Terraform Provider](https://registry.terraform.io/providers/dynatrace-oss/dynatrace/latest)
    - [Extend OneAgent to instrument a non-native language through the OneAgent SDK](https://docs.dynatrace.com/docs/extend-dynatrace/extend-tracing/oneagent-sdk)
    - [Service Now Integrations](https://docs.dynatrace.com/docs/observe-and-explore/notifications-and-alerting/problem-notifications/servicenow-integration)
    - [Setup BizEvents](https://docs.dynatrace.com/docs/platform-modules/business-analytics/ba-events-capturing)
 

1. Presentation Overview

    Again, your presentation should highlight your technical aptitude by demonstrating the core concepts and feature functionality of the tool. However, the primary focus of your presentation will be to demonstrate the value of the data provided by Dynatrace to multiple business units, teams and stakeholders for any given organization. For the purposes of this demo the Dynatrace Sales Engineering team will be role playing as stake holders of a prospect in the roles of:  
    
    - Technology Operations
    - C Level Management
    - Software Development
    - DevOps
    - SRE
    - Infrastructure Support
    - Business Analytics & Intelligence

    Tailor your presentation to demonstrate how each of these teams day-to-day jobs could be easier and drive better business outcomes with the Dynatrace platform. Additionally, be prepared to field live questions from these business units' stakeholders about the Dynatrace platform from their specific lens. 

1. Presentation requirements: 

    - Present a problem card and the related application, user, service and business impact 
    - Build a dashboard that showcases your environment and it's data
    - Explain the value of the [Dynatrace Smartscape](https://docs.dynatrace.com/docs/platform/smartscape)
    - Walk through the application service flow you've instrumented with one agent from front end (Real users) to the database calls
    - Highlight 5 data points or features or learned about during setup
    - Explain why these 5 data points are relevant to the audience & business units 
    - Demo the 2 (or more) integrations you setup
    - Present one item from your environment under ["Profiling and Optimization"](https://docs.dynatrace.com/docs/platform-modules/applications-and-microservices/profiling-and-optimization) or ["Multidimensional Analysis"](https://docs.dynatrace.com/docs/platform-modules/applications-and-microservices/multidimensional-analysis)
    - The over arching theme of your presentation should hinge of the business value the above requirements will provide to your prospect

    Additional Notes:

    - Please Ensure that you have enabled [Real User Monitoring (RUM)](https://docs.dynatrace.com/docs/platform-modules/digital-experience/web-applications/initial-setup/configure-dynatrace-real-user-monitoring-to-capture-xhr-actions) for you web app
    - If you use the standalone version of Easy Travel you may need to [configure custom service detection](https://docs.dynatrace.com/docs/platform-modules/applications-and-microservices/services/service-detection-and-naming/service-types/custom-services)
    - Please make sure you disable injection the launcher process / docker container for easy travel. [See related documentation here](https://community.dynatrace.com/t5/Getting-started/easyTravel-Documentation-and-Download/td-p/181271)
    - [Take a look at YouTube for Sample Demos](https://www.youtube.com/results?search_query=dynatrace+demo)
    - Feel free to 
    - Have fun!
    
