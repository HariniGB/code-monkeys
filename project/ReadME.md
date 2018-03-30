# S3URL
> S3URL application shortens, saves and share your URLs with the world. Generated URLs can seamlessly be shared on social media platforms like Twitter and tracked/managed in the “My account” page. The simplicity of S3URL is powered under the hood by cutting edge technology.  S3URL completely runs in a self-managing environment with the help of Kubernetes. The entire fleet of micro services are run as Docker containers inside of Kubernetes. At S3URL we are big believers of CI/CD and we use Fabric8 for just that. Whenever code is checked into our source repositories, it is automatically pulled by Jenkins, tested and deployed to staging servers.The entire system is monitored using Prometheus and centralized dashboards show the behavior of all the micro services. PagerDuty integration makes sure that we are alerted immediately when an issue occurs so that we can jump on it. Centralized logging through BEK (Beats, Elasticsearch, Kibana) helps our developers to rapidly debug issues that are reported by customers. Our NoSQL databases are built to scale for any number of customers that come on board. The entire experience for customers and developers is backed by our intuitive SSO that can expose different role based views.
[![S3URL-Home](https://i.imgur.com/3SPukbI.png)](https://i.imgur.com/3SPukbI.png)


## User Interfaces
>S3URL allows both user and developers to Signup a new account and login at anytime. It also provides an essential facility for users to maintain their related data in their profile. The My account page allows the user to keep track of all their long URLs with their generated shorten URLs and date on which they generated it. In addition to this user interface facility, we have also implemented a place where the users can share their URLs to their tweeter account. They can edit their post if required. On the other hand, the graphic user interface is completely build using HTML, CSS,JS and made responsive to adjust the layout for different machine sizes. The developers also maintain an account  where they are provided to Single Sign On in to both Jenkins and the Gogs in order to reduce their valuable time in creating accounts, signing in with different usernames and so on. Moreover, the developers are authorized to maintain the source code and keep an update on the testing pipeline in Jenkins. The main feature is Shorten URL. The user interface provides the users a simple text box with a one click button that generates the required shorten URL and records the time and details to the user profile. It is simple and secure. Overtime the user clicks the shorten URL, the URL automatically redirects to the original link. This reduces the pressure in the minds of the users to remember a long hashed URL and  helps them to save their URLs for future reference.


[![S3URL-SSO](https://i.imgur.com/jFHy9Fx.jpg)](https://i.imgur.com/jFHy9Fx.jpg)


## Hardware Interfaces
> This application is a simple web application which needs a web browser to run. We have used golang to implement the URL shorten APIs and Single Sign On for developers. We have to run the application in the go server. The softwares we have used can be configured in the localhost or with a public domain. This other tools like Prometheus, Pager-duty, Elastic search, Beats, Kibana, Grafana and Fabric8 are completely based on one time configuration in their portals and continuous integration and delivery of the jenkins pipeline.


[![Grafana](https://i.imgur.com/5hwfboi.png)](https://i.imgur.com/5hwfboi.png)

[![Kibana](https://i.imgur.com/jV16D5a.png)](https://i.imgur.com/jV16D5a.png)


## Software Interfaces
> S3URL web application is build using golang and run on the go server. We have implemented the Single Sign On feature which is configured using LDAP (Lightweight Directory Access Protocol) that runs above the TCP/IP stack layer in order to connect to or modify the directories in the internet. LDAP is configured in a ubuntu server using a VM (virtual machine). We have used NoSQL databases to scale for any number of customers that come on board. Reverse Proxy server that is located behind the firewall in a our network directs the user login credentials to the  gogs and Jenkins server to allow single sign on ability. The entire web application is deployed as docker containers with kubernetes on Fabric8. Fabric8 proves an end to end development platform in which our S3URL can be build, tested and deployed with CI/CD.
[![Fabric8](https://i.imgur.com/6WMJZui.png)](https://i.imgur.com/6WMJZui.png)

## Communications Interfaces
> The application entirely communicates using REST APIs for shorten URL service, LDAP for user login credentials which are saved in mongoDB. Our application is build as micro services to leverage the loosely coupled capabilities and allows continuous integration and delivery. We used OpenLDAP a directory service to configure LDAP in an ubuntu server. The LDAP that runs above the TCP/IP stack layer allows to create users in a group as well. The ldap.conf file need to be configured using the database name, vm location, organization name and password. We have used Reverse proxy server to accelerate the performance by compressed inbound and outbound traffic data and also provides header for backend servers which acts as a defense against security treats/attacks. Using this proxy server we have leveraged the single sign on feature with jenkins, gogs and fabric8. Fabric8 acts as a single platform that merges the functionality of several other tools like Grafana, Kibana, Prometheus, Metrics, Gogs and Jenkins. We used gofabric8 to validate and deploy fabric8 components on to the Kubernetes environment. We used minikube  to view the fabric8 user interactive dashboard. We can view the entire building and testing pipeline in this dashboard.
[![S3URL](https://i.imgur.com/qXh3qKQ.png)](https://i.imgur.com/qXh3qKQ.png)

## Project Accomplishments

>S3URL comes with a clean and simple interface to create, manage and share URLs. It is done both through a user interface and REST APIs. Angular.js helps us to deliver an experience that is clean, seamless and. Generated URLs can seamlessly be shared on social media platforms like Twitter and tracked/managed in the “User dashboard” page. The simplicity of S3URL is powered under the hood by cutting edge technology.  S3URL completely runs in a self-managing environment with the help of Kubernetes. The entire fleet of micro services are run as Docker containers inside of Kubernetes. At S3URL we are big believers of CI/CD and we use Fabric8 for just that. Whenever code is checked into our source repositories, it is automatically pulled by Jenkins, tested and deployed to staging servers. The entire system is monitored using Prometheus and centralized dashboards show the behavior of all the micro services. PagerDuty integration makes sure that we are alerted immediately when an issue occurs so that we can jump on it. Centralized logging through BEK (Beats, Elastic search, Kibana) helps our developers to rapidly debug issues that are reported by customers. Our NoSQL databases are built to scale for any number of customers that come on board. The entire experience for customers and developers is backed by our intuitive SSO that can expose different role based views. S3URL is built for scalability, reliability and high availability. If you believe in our vision, then go ahead and tap on the “Donate now” to donate via PayPal. List of features we have accomplished with application. 

[![Jenkins](https://i.imgur.com/mtuBIN3.png)](https://i.imgur.com/mtuBIN3.png)

- SSO based on Nginx reverse proxy.
- Micro-service that shortens long URL.
- Micro-service that redirects web traffic.
- Run infrastructure on the Kubernetes.
- CI/CD is achieved via Fabric8 & Jenkins.
- Twitter and PayPal integration



## Reference
- https://fabric8.io/docs
- https://www.linuxbabe.com/ubuntu/install-configure-openldap-server-ubuntu-16-04
- https://help.ubuntu.com/lts/serverguide/openldap-server.html#openldap-server-postinstall
- http://www.zytrax.com/books/ldap/ch11/groups.html

## Appendix

### Appendix A: Glossary
S3URL(shortens, saves and share your URL), Fabric8, Docker, Kubernetes, Prometheus, Elastic search, Beats, Kibana, Grafana, PagerDuty, LDAP (Lightweight Directory Access Protocol), SSO (Single-Sign-On), Jenkins, Gogs.

### Appendix B: Demonstration Link 
Youtube URL:     https://youtu.be/YzUjwCK1hpA
Google Drive URL:       https://drive.google.com/file/d/1hHswknjABqMUsUS3cCJE2PZHnGUiprSS/view?usp=sharing



