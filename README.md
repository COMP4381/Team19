# Tourist Attraction

## Motivation
The problem domain is tourism (searching a restaurant to eating), the speicific SOA-based solution under this domain is searches for the nearest restaurant from your location to eat, because A large number of people benefit from growth, because easier to use, cheaper solution, better maintenance, the value add is nearest restaurant from the user.
## Service Design
## SOA Diagram
![soa diagram](https://user-images.githubusercontent.com/44411022/49698719-4233af00-fb7c-11e8-95a7-235132dfa9e7.png)

the three tiers in this 3-tier client server architecturethe is Model View Controller (MVC) and the clients is users and the services is google places,google distance matrix, Web server and the atomic service is google places,google distance matrix and the composite is Web server.


## BPMN 2.0 Diagram 
![untitled diagram](https://user-images.githubusercontent.com/44411022/49698740-ace4ea80-fb7c-11e8-9825-6561692f7431.png)

The compiste service get location from user after that request the location to the google places and the google places return jason respons of nearest restaurant to compiste service after than request user location and restaurant location to distance matrix after
that return jason respons to the compiste service and compiste service compute and return  the less distance of restaurant to user.

## Implementation Details.
We impelemented our services using the RESTful service development paradigm. Which is based on the HTTP protocol which is an RPC-based synchronous communication protocol.
## Composite Service Algorithm According to BPMN 2.0.
![image](https://user-images.githubusercontent.com/34231700/50542680-edf47b80-0bcb-11e9-8d1e-8ac16427a94f.png)
## Applied Technologies.
 ###### development environment: Eclipse. 
 ###### programming languages:Java.
 ###### frameworks and libraries:swagger, spring boot.
 ###### Google provider.
 ###### application server:Apach Tomcat.
 

 
 
 
 
 
 ## Design Patterns.
 ### Exception Design Patterns.
 ##
 ![design pattren](https://user-images.githubusercontent.com/44411022/50542821-1c963600-0b7b-11e9-91f8-f307b9eee570.png)
 










##abstract
Tourist need to eat in city dont know anything about this city 
he dont konw where to go to eat  so will use this mobile application 
to find resturant and how distance should be travel and how take time and something to direcit him to 
the location of resturant 

1-open this apps
2-search for resturant or name of restrant he want 
3- if resturant avalabil then will tell him the distance and time need to arrive and direct him 
if he dont know name of resturant so will suggest some name of resturant depends his location by using Gps
we use these atomic services  places api ,matrix api ,dirction api and Gps help also
## 
## SOA Architecture
![soa diagram](https://user-images.githubusercontent.com/44411022/49698719-4233af00-fb7c-11e8-95a7-235132dfa9e7.png)

##
## BPMN 
![untitled diagram](https://user-images.githubusercontent.com/44411022/49698740-ace4ea80-fb7c-11e8-9825-6561692f7431.png)
