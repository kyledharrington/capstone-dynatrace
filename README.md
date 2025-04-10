# Solutions Engineering Capstone

Thank you for your interest in being a part of the Solutions Engineering team at Dynatrace. As next steps we will ask you to setup and demo an environment of your choosing to the Solutions Engineering team, instrumented by the Dynatrace platform. The goal of this capstone is to showcase your technical skills, the core features of the Dynatrace platform, and your ability to present its value to various business units in one presentation.

See below for further instructions and expectations of this demo and reach out to your hiring manager or kyle.harrington@dynatrace.com with any questions.
    - If you are planning on using a Dynatrace Managed install for this demo, please see the [Dynatrace Managed Capstone](/dt-managed/dt-managed-capstone.md) for instructions

1. Sign up for a free Dynatrace SaaS trial 
    - https://www.dynatrace.com/trial/

1. Deploy OneAgent to your environment
    - [Linux](https://docs.dynatrace.com/docs/setup-and-configuration/dynatrace-oneagent/installation-and-operation/linux/installation/install-oneagent-on-linux)
    - [Windows](https://docs.dynatrace.com/docs/setup-and-configuration/dynatrace-oneagent/installation-and-operation/windows/installation/install-oneagent-on-windows)
    - [Kubernetes / OpenShift - Helm](https://docs.dynatrace.com/docs/ingest-from/setup-on-k8s/deployment/full-stack-observability)
    - [Kubernetes / OpenShift - Manifest Deployment](https://docs.dynatrace.com/docs/shortlink/installation-k8s-cloud-native-fs#manifest)

1. Deploy a Web Application
    
    Setup a demo application into your environment.

    Requirements of the demo application 
    - Front end web server (for browser RUM injection) 
    - Code level calls more advance than a "hello world" or health check 
      -  Check [Dynatrace's list of supported technologies](https://docs.dynatrace.com/docs/setup-and-configuration/technology-support) for technology compatibility
    - Application logs are generated and available (stdout by default)
    - A Database component 
    - The application must be capable of generating errors/ crashes/ outages

    Any application that meets the requirements section above will work. You can choose any custom application you have worked with in the past or built for this demo. See below for a list of sample apps you can potentially leverage and will meet the requirements. 

    - [Astronomy Shop](https://opentelemetry.io/docs/demo/kubernetes-deployment/)
    - [Online Boutique](https://github.com/GoogleCloudPlatform/microservices-demo)
    - [Easy Travel - Standalone](https://community.dynatrace.com/t5/Getting-started/easyTravel-Documentation-and-Download/td-p/181271)
    - [Easy Travel - Docker](https://github.com/Dynatrace/easyTravel-Docker)

    
1. Configuration requirements:

    Below is a list of the requirements needed to be done to your Dynatrace environment as well as documentation links to get you started. These are intended to be challenging and highlight how your previous experience will translate to Dynatrace's Solutions Engineering team. While the Dynatrace documentation links are included, please note, these are only examples and are not specific to any demo application. There are many ways to ingest and configure data in Dynatrace.

    Required Configurations for your Demo

    Administration     
    
    - [Setup Tagging Rules for your environment](https://docs.dynatrace.com/docs/manage/tags-and-metadata/setup/how-to-define-tags)
    - [Configure a outbound problem notification via Workflows](https://docs.dynatrace.com/docs/analyze-explore-automate/workflows/simple-workflow)
    - [Create a segment to organize your infrastructure or data](https://docs.dynatrace.com/docs/manage/access-control/management-zones/set-up-management-zones)
    

    Observability
    - [Logs Ingestion](https://docs.dynatrace.com/docs/analyze-explore-automate/logs/lma-log-ingestion)
    - [Metric Ingestion](https://docs.dynatrace.com/docs/analyze-explore-automate/metrics)
    - [Trace Ingestion](https://docs.dynatrace.com/docs/analyze-explore-automate/distributed-tracing/ingest-traces)

    Real User Monitoring
     - [Add a browser monitoring check to your web application](https://docs.dynatrace.com/docs/observe/digital-experience/synthetic-monitoring/browser-monitors/create-a-single-url-browser-monitor)
    - [Enable Session Replay Capture](https://docs.dynatrace.com/docs/platform-modules/digital-experience/session-replay/enable-session-replay-web)
    - [Configure conversion goals for your web application](https://docs.dynatrace.com/docs/platform-modules/digital-experience/web-applications/analyze-and-use/define-conversion-goals)
   
 
1. Additional configuration recommendations
    
    These are not required, but it is strongly encouraged that you configure some of these. Make sure you call these out during your demo if you set them up!

    - [BizEvents](https://docs.dynatrace.com/docs/platform-modules/business-analytics/ba-events-capturing)
    - [Log Events](https://docs.dynatrace.com/docs/analyze-explore-automate/logs/lma-analysis/lma-log-events) 
    - [Live Debugger](https://docs.dynatrace.com/docs/observe/applications-and-microservices/developer-observability/offering-capabilities)
    - [RUM Session Properties](https://docs.dynatrace.com/docs/platform-modules/digital-experience/web-applications/additional-configuration/define-user-action-and-session-properties)
    - [OpenTelemetry Ingestion](https://docs.dynatrace.com/docs/ingest-from/opentelemetry)
    - [Run Time Vulnerabilites](https://docs.dynatrace.com/docs/secure/application-security/vulnerability-analytics)
    - [Kubernetes Security Posture Management](https://docs.dynatrace.com/docs/ingest-from/setup-on-k8s/deployment/security-posture-management)
    - [Metric Ingestion](https://docs.dynatrace.com/docs/extend-dynatrace/extend-metrics/ingestion-methods/oneagent-metric-api)
    - [Dynatrace Co-Pilot](https://docs.dynatrace.com/docs/discover-dynatrace/platform/davis-ai/copilot/copilot-getting-started)
    - [Add a Synthetic check to you web app via a *Private* active gate](https://docs.dynatrace.com/docs/platform-modules/digital-experience/synthetic-monitoring/private-synthetic-locations/create-a-private-synthetic-location)
    - [Use the Events API to add Event data to a Dynatrace entity](https://docs.dynatrace.com/docs/dynatrace-api/environment-api/events-v2/post-event)
    - [Integrate Dynatrace with a Cloud Account](https://docs.dynatrace.com/docs/platform-modules/infrastructure-monitoring/cloud-platform-monitoring)
    - [Leverage the Dynatrace Terraform Provider](https://registry.terraform.io/providers/dynatrace-oss/dynatrace/latest)
    - [Extend OneAgent to instrument a non-native language through the OneAgent SDK](https://docs.dynatrace.com/docs/extend-dynatrace/extend-tracing/oneagent-sdk)
    - [Instrument a Python application with OneAgent](https://github.com/dynatrace-oss/OneAgent-SDK-Python-AutoInstrumentation)

    Feel free to review the full Dynatrace product documentation on [Getting started with Dynatrace](https://docs.dynatrace.com/docs/get-started) and [Product News](https://www.dynatrace.com/news/blog/) pages and come up with your own integration ideas for you demo.
 

1. Presentation Overview

    Your presentation should highlight your technical aptitude by demonstrating the core concepts and feature functionality of the tool. However, the primary focus of your presentation will be to demonstrate the value of the data provided by Dynatrace to multiple business units, teams and stakeholders for any given organization. For the purposes of this demo the Dynatrace Solutions Engineering team will be role playing as stake holders of a prospect in the roles of:  
    
    - C Suite Leadership 
    - Technology Operations
    - Software Development
    - DevOps
    - Site Reliability Engineer
    - Infrastructure Support
    - Business Analytics & Intelligence
    - etc

    Come prepared with these roles in mind and tailor your presentation to demonstrate how each of these teams day-to-day jobs could be different and drive better business outcomes with the Dynatrace platform. Additionally, be prepared to field live questions from these business units' stakeholders about the Dynatrace platform from their specific lens. 

1. Presentation requirements: 

    Below is a list of the required features, applications and/or functionality of the Dynatrace platform which need to be incorporated into your demo. 

    Dynatrace Apps 
    - [Problems App](https://www.dynatrace.com/hub/detail/problems/)
    - [Infrastructure and Operations](https://www.dynatrace.com/hub/detail/infrastructure-operations)
    - [Logs App](https://www.dynatrace.com/hub/detail/logs/) 
    - [Traces app](https://www.dynatrace.com/hub/detail/distributed-tracing)
    - [Services App](https://www.dynatrace.com/hub/detail/services-1/)
    - [Kubernetes App](https://www.dynatrace.com/hub/detail/kubernetes-1) (if you leveraged Kubernetes)
    - [Dynatrace Smartscape](https://docs.dynatrace.com/docs/platform/smartscape)

    Features 
    - [Dynatrace Query Language (DQL)](https://docs.dynatrace.com/docs/discover-dynatrace/references/dynatrace-query-language)
    - [The configured Tagging Rules](https://docs.dynatrace.com/docs/manage/tags-and-metadata/setup/how-to-define-tags)
    - [The configured outbound problem notification via Workflows](https://docs.dynatrace.com/docs/analyze-explore-automate/workflows/simple-workflow)
    - [The configured segment(s) to organize your infrastructure or data](https://docs.dynatrace.com/docs/manage/access-control/management-zones/set-up-management-zones)
    - [The configured browser monitoring check to your web application](https://docs.dynatrace.com/docs/observe/digital-experience/synthetic-monitoring/browser-monitors/create-a-single-url-browser-monitor)
    - [The configured Session Replay Sessions](https://docs.dynatrace.com/docs/platform-modules/digital-experience/session-replay/enable-session-replay-web)
    - [The configured conversion goals for your web application](https://docs.dynatrace.com/docs/platform-modules/digital-experience/web-applications/analyze-and-use/define-conversion-goals)
    
    Demo Expectations
    - All of the above "Dynatrace apps" and "features" are incorporated into you demo
    - Present a problem card generated in your environment and the related application, user, service and business impact 
    - Build a dashboard that showcases your environment and it's data via the [Dashboard app](https://www.dynatrace.com/hub/detail/dashboards/)
    - Walk through the application service flow you've instrumented with one agent from front end (Real users) to the backend (database calls)
    - Highlight the value of the data provided by the Dynatrace platform to your audience
    - Incorporate how you would benefit from the Dynatrace platform & data you are presenting in your current or previous role(s) 

    Tips for success:

     The over arching theme of your presentation should hinge of the business value the above requirements will provide to your audience. Focus on business value  highlighting how the Dynatrace platform can drive revenue, reduce costs, or improve efficiency.

    - Get to know your audience. Understand the background of your audience to tailor the narrative and depth of your demo.
    - Highlight just the key features. Focus on the most important technical features and how they work, but avoid a "feature demo" 
    - Articulate the practical application of the platform. Explain how the technical features solve real-world problems for your audience.
    - Be prepared for questions & interruptions from you audience
    - Try to maintain engagement. Keep the audience engaged with interaction and encourage questions throughout the demo.

        
    If you need additional ideas for demos, talking points or general knowledge take a look at:
    - [Dynatrace YouTube Channel](https://www.youtube.com/@dynatrace)
    - [Dynatrace LinkedIn](https://www.linkedin.com/company/dynatrace/posts/?feedView=all)
    - [Dynatrace Playground SaaS Environment](https://wkf10640.apps.dynatrace.com/)
    - [Dynatrace Blog](https://www.dynatrace.com/news/blog/)

   
    Additional Notes:
    - Please Ensure that you have enabled [Real User Monitoring (RUM)](https://docs.dynatrace.com/docs/platform-modules/digital-experience/web-applications/initial-setup/configure-dynatrace-real-user-monitoring-to-capture-xhr-actions) for you web app
    - If you use the standalone version of Easy Travel you may need to [configure custom service detection](https://docs.dynatrace.com/docs/platform-modules/applications-and-microservices/services/service-detection-and-naming/service-types/custom-services)
    - Please make sure you disable injection the launcher process / docker container for easy travel. [See related documentation here](https://community.dynatrace.com/t5/Getting-started/easyTravel-Documentation-and-Download/td-p/181271)
     - Have fun!