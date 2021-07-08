# System Design Laboratory
This is a comprehensive documentation of various aspects of software system designing. We will be covering the basic bare minimum aspects of software designing based on a different category. Later we will pick few of the already available systems from a different category to come up with the detailed system design on which the product/ service can be build. This would be a good start for job seekers for practicing and understanding system designing concepts.

When ever you start designing a system, it's very much required to understand few details about the systems. To understand the system you should ask following few questions.

1. What is it for? 
2. Who are the targeted customer? 
3. How does it solve the problem?
5. What is the product road map?

## System Requirements
Once you understand the basics of the system, it's important to clarify what are actual use cases and requirements. While you are documenting the functional requirements be sure to document non-functional and extended requirements also. It's very important to design a system for a given scope.

## Capacity Planning
The very next thing you have to confirm is the capacity. while there would be different strategies can be adapted based on the type of system, we will consider a simple API system to understand it more.

### Traffic Estimates
The best way to start capacity planning by estimating the traffic to the system. You should understand the overall load for your system based on the different use cases and put up a figure which should be the traffic per second. It would be helpful to come up with the ratio between traffics of different use cases. This would help you in choosing right database strategy for your system.

### Storage Estimates
Now once you have the traffic estimates for your system, so you can come up with the storage requirement for all your use cases and can put up a figure based on your requirement and purging strategy. 

### Bandwidth Estimates
With the above two estimates and with some maths you can come up with bandwidth estimation for your system for all your use cases.

### Memory Estimates
If you estimate your system going to face a heavy traffic, be sure to consider on the performance aspect of it. Caching is once of the technique widely used for improving application performance. In this case do not forget to put the Memory estimates.

Once all the estimates are done. It's good to provide a summery for a quick reference.

## System Functionalities Or APIs
Now we are good to design the system functionalities or APIs based on the use cases. It's important to clearly document the input and output of the functions or APIs. Some people even document the datatype for those.

## Abstract Design
Draw all the primary components of the system for a high level understanding. You should include load balancers, primary and slave nodes for databases/caching systems etc.

## Database Design
Database designing is very crucial, so it's very important you understand your data model well and chose the right database based on the use case. Following are the few aspects that I consider while picking the right database.

1. Is there a lot of relations defined between entities of your system?
   This will help you to consider a relational or a NoSQL database.
2. What is your storage requirement?
   If you are expecting billions data, consider having a distributed database.
3. Security needs about the data. Check if the data has to be encrypted or not.     
   
Always consider documenting partitioning of the tables for scalability and performance.

### Database Schema
Once you are good with requirements and overall design you should now able to put a data model for you system.

## Detailed Design
While it's not necessary to document all the components of your system, but it's good to document the low level details about few of the important components and decision makings. While you put this details it's good to consider memory, cpu, concurrency etc. You should document specific bottlenecks and resolutions for them.

## Availability & Reliability
You should consider following points also in your design.

1. Horizontal Scaling by adding more nodes for a service and served the service via load balancer
2. Data Replication to avoid any single point of failure
3. Cluster solutions to recover automatically in case of any failure

## Purging And Clean up
In any system we should always think of data purging and clean up. This is very necessary for a software system. You should always find out appropriate business use cases for this.

## Security And Permissions
Last but not least, you should always consider security and permission requirements. 

## Analytics
Now when we are living in a world where data is very crucial, you should always consider AI, ML opportunities on the data that your system deal with.

## System Design Bucket

* [Tiny URL](tiny-url)




