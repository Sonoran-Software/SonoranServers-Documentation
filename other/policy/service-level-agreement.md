---
description: View the Service Level Agreement for Sonoran Servers.
---

# Service Level Agreement

This Service Level Agreement (“SLA”) is a policy governing the use of the services between Sonoran Software Systems LLC (“Company”) and Customers. Customer must read, agree with and accept all of the terms and conditions contained in this Agreement. The Company may amend this Agreement at any time by posting a revised version on its website

## 1. Services.

For purposes of this Agreement, the services to be provided by the Company (“Services”) are those services which Customer requested be supplied by the Company and for which Customer agreed to pay based on Customer’s clicking through the options on the Company’s website.

## **2. Technical Support.**

The Company provides Customer with technical support on setup of Customer’s account on one or more of the Company’s servers, access, and other server related issues to the primary technical contact free of charge. The Company does not provide support for web applications, third party software, scripts, or components from third parties or developed by Customer.

The Company’s servers are monitored 24 hours per day, 7 days per week, 365 days per year and support agents are available by ticketing system as posted in the support section of the Company’s website.  Please send us a message with the full description of the problem and Customer’s account username. Please do not send multiple messages on the same issue. &#x20;

## 3.  Billing and other account-related inquiries.

All inquiries regarding the Company’s billing for its services should be sent via our ticketing system.

All inquiries regarding reselling the Company’s services, purchasing of new accounts and available discounts should be addressed to the ticketing system found on the Company’s website.

## 4.  Escalation.

If Customer is dissatisfied with the Company’s Service or if Customer is unable to resolve a technical support issue within the parameters outlined in this Agreement please contact the Company. The Company will review Customer’s concerns, investigate, and respond to Customer within one (1) business day. As issues may be complex or require extensive investigation, the foregoing response time does not imply that a resolution is guaranteed within said one (1) business day.\


## 5.  Online tools, control panel, and server management.

Customer is provided with certain online tools, and the Company expects Customer to use these tools to perform all available account and server management tasks.

These tools, together with server management documentation and help, are available online at the support section of the Company’s website.  If Customer experiences difficulty using these tools, the Company’s technical support personnel will help Customer learn how to use these tools. However, the Company’s technical support personnel shall not be expected to perform for Customer the tasks that can be done through the available tools.

## 6.  Servers Availability.

The Company is fully committed to providing quality service to all customers. To support this commitment, the Company provides the following commitments and tools related to this Agreement.

## 6.1  Application (Web) Server.

(a)  Availability.  The Company guarantees a 99.9% monthly average of scheduled availability of its Application (Web) Servers. Application (Web) Server availability is defined as Customer’s ability, via web browser, to retrieve the HTTP headers from a hosting server. The Company does not monitor availability of individual web sites but only monitors the server availability as a whole.

(b)  Monitoring.  To verify that the server is available, the Company will ping the HTTP service on the server by retrieving HTTP headers every minute. If an HTTP service does not respond, the server is considered non-operational and is manually rebooted. If rebooting the server does not solve the problem, it is immediately escalated to the Support Center.

In cases where two or more consecutive HTTP tests fail, the server downtime will be registered as the number of minutes between the first and the last failed tests. Downtime of less than 5 minutes in duration is not recorded. The Company calculates server uptime based on this type of server monitoring.

##

## 6.2  Mail Server.

(a)  Availability.  The Company guarantees a 99.9% monthly average of scheduled availability of its mail servers. Mail server availability is defined as the client’s ability to send (SMTP) and retrieve (POP3) e-mail via the particular mail server. The Company does not monitor individual mail accounts, but only monitors the server as a whole. Mail server unavailability caused by denial of service attacks, mail bombing, and other flooding techniques is not included in uptime calculations.

Mail delivery protocol (SMTP) is a “store-and-forward” type of protocol that does not guarantee immediate delivery of e-mail messages. In the case that the first delivery attempt is failed, the mail server will continue to attempt to deliver messages to the addressee according to a predefined schedule. In the case that the messages cannot be delivered for a period of time exceeding 48 to 72 hours, the messages are returned to the sender.

(b)  Monitoring.  To verify that the server is available, the Company will ping the SMTP and POP services (retrieve SMTP and POP headers) every minute. If either service does not respond, the service is considered non-operational and is automatically restarted. If two or more consecutive SMTP or POP tests fail, the problem is immediately escalated to the Support Center.

In cases where two or more consecutive SMTP or POP tests fail, the server downtime will be registered as the number of minutes between the first and the last failed tests. Downtime of less than 5 minutes in duration is not recorded. The Company calculates server uptime based on this type of server monitoring.

## 6.3  Network Availability.

Network availability is defined as the Company’s network’s ability to pass incoming and outgoing TCP/IP traffic. A server’s unavailability caused by network unavailability is not included in server uptime. Interruptions of service due to problems on the backbone or on the Customer’s portion of the network are beyond the Company’s control and are not included in uptime calculations. Interruptions of service caused by denial of service or similar attacks are beyond the Company’s control and are not included in uptime calculations.

## 6.4  Scheduled Maintenance.

To guarantee optimal performance of the servers, the Company will perform maintenance on the servers on a routine basis. Such maintenance often requires taking Company servers off-line. Company reserves two hours of server unavailability per month for maintenance purposes. This server unavailability is not included in server uptime calculations. The maintenance typically is performed during off-peak hours. Company provides Customer with advance notice of maintenance whenever possible.

## 6.5  Hypervisor Availability

(a)  Availability.  The Company guarantees a 99.9% monthly average of scheduled availability of its Hypervisors and relative services. Hypervisor availability is defined as Customer’s ability, via web browser to the connection of Company hypervisor control panel. The Company does not monitor the availability of individual servers but only monitors the node's availability as a whole.

(b)  Monitoring.  To verify that the server is available, the Company will ping the HTTP service on the node by retrieving HTTP headers every minute. If an HTTP service does not respond, the server is considered non-operational and is manually rebooted. If rebooting the server does not solve the problem, it is immediately escalated to the Support Center.

In cases where two or more consecutive HTTP tests fail, the server downtime will be registered as the number of minutes between the first and the last failed tests. Downtime of less than 5 minutes in duration is not recorded. The Company calculates server uptime based on this type of server monitoring.

## 7.  Server Storage Capacity.

Each account is allotted storage capacity on the Company’s servers according to the plan or options selected by Customer. This storage size can be increased through the online control panel for an additional charge up to the maximum amount allowed for each plan or service, as described on the Company’s website. The servers may stop accepting, processing, or delivering data when the purchased limit is reached, thus causing server unavailability or data loss. The Company shall not be held responsible for such unavailability or data losses.

## 8.  Customer Responsibilities.

To access the Company Services Customer must provide to the Company the following minimum requirements:

(a)  an Internet connection with sufficient bandwidth and quality to allow trouble-free browsing and data uploading and downloading;

(b)  a fully functional Internet browser;

(c)  a fully functional POP/SMTP e-mail program (client);

(d)  tools to develop and publish content as Customer deems necessary;

(e)  tools to access database servers if such services are purchased by Customer as part of the Services.

## 9.  Requesting Service Credits.

Service Credits may be awarded in the following scenarios as outlined in this SLA:

1. Any unplanned outage on a Game Server, Virtual Private Server, Dedicated Server, or Web Hosting node.
2. A network interruption of greater than ten (10) minutes on a Virtual Private Server, Dedicated Server, or Web Hosting node.
3. Distributed Denial of Service (DDoS) attack on Sonoran Server's hardware, server(s), or infrastructure;
4. Any other unplanned or unannounced interruption of service on a Virtual Private Server, Dedicated Server, or Web Hosting node.

If the client feels that you are entitled to service credits as outlined in the above section, the following procedures must be followed to obtain such service credits:

A support ticket must be opened via our customer support service at support.sonoransoftware.com

Service Credits must be redeemed 72 hours from the incident or posting of an official post-mortem announcement from Sonoran Software Systems LLC

The ticket must contain the service name, outage time, and total affected duration.

Any other relevant information that could prove helpful to our team issuing service credits.\


## 10.  Service Credit Calculation.

Service Credits are time-based credits and are calculated in a standard proportional manner, by taking the length of credited time and dividing it by the length of the service period, then multiplying by the cost of the service per period. For instance, if a service costing 1000 USD per month were to suffer one hour of network downtime, the monetary credit would be (1 hr)/(24 hours \* 30 days) \* (1000 USD), or 1.39 USD.

For intermittent outages, Sonoran Software Systems LLC reserves the right to determine if a period of time between short outages qualifys for SLA credits in addition to the base outage duration.\
