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
 ## Service Deployment and Monitoring.
 ## Log file.
 *https://github.com/COMP4381/Team19/blob/master/Logs%20file.csv*
## Conclusion and Discussion.
the project is not hard but the hard in this project is how to obtain key from google because the key run one time to test because this problem i requested more than 25 key for test the project.
 ## Design Patterns.
 ### Exception Design Patterns.
 ##
 ![design pattren](https://user-images.githubusercontent.com/44411022/50542821-1c963600-0b7b-11e9-91f8-f307b9eee570.png)
 
 ## Inventory: Service layers
 ![src_main](https://user-images.githubusercontent.com/44411022/50542850-6a5f6e00-0b7c-11e9-9bb7-168ca784eecc.png)
 # Service Monitoring.
 the all APIs is 
 ![all api dashbord](https://user-images.githubusercontent.com/34231700/50551352-d4b10500-0c87-11e9-9bd9-d476c8309a59.PNG)
 ## google places.
 ![api traffic](https://user-images.githubusercontent.com/34231700/50550742-6b78c400-0c7e-11e9-8880-b3795cd3214d.PNG)
*https://github.com/COMP4381/Team19/blob/master/places%20traffic.csv*
![api error](https://user-images.githubusercontent.com/34231700/50550758-aaa71500-0c7e-11e9-87a7-d22cdf8b7772.PNG)
*https://github.com/COMP4381/Team19/blob/master/places%20errors.csv*
 ## google distance matrix.
 ![matrix trafic](https://user-images.githubusercontent.com/34231700/50550820-8bf54e00-0c7f-11e9-8342-79f1b25d7833.PNG)
*https://github.com/COMP4381/Team19/blob/master/matrix%20traffic.csv*
![matrix error](https://user-images.githubusercontent.com/34231700/50550852-fdcd9780-0c7f-11e9-8997-1c5d9bbb862f.PNG)
*https://github.com/COMP4381/Team19/blob/master/matrix%20errors.csv*
![matrix latency](https://user-images.githubusercontent.com/34231700/50550856-0a51f000-0c80-11e9-813e-527b20f64453.PNG)
*https://github.com/COMP4381/Team19/blob/master/matrix%20latency.csv*
 ## APPENDIX
 ### Documentation for API Endpoints.
 #### CompositeServiceControllerApi
All URIs are relative to *https://localhost:8090*

Method | HTTP request | Description
------------- | ------------- | -------------
[**findPlaceUsingGET**](CompositeControllerApi.md#findPlaceUsingGET) | **GET** /Composite | findPlace
##
## Atomic Controllers.
#### UserControllerApi.

All URIs are relative to *https://localhost:8090*

Method | HTTP request | Description
------------- | ------------- | -------------
[**adduserUsingPOST**](UserControllerApi.md#adduserUsingPOST) | **POST** /user/user | adduser
[**finduserByNameUsingGET**](UserControllerApi.md#finduserByNameUsingGET) | **GET** /user/user | finduserByName
[**getUserUsingGET**](UserControllerApi.md#getUserUsingGET) | **GET** /user | user
[**getuserByIDUsingGET**](UserControllerApi.md#getuserByIDUsingGET) | **GET** /user/user/{id} | getUserByID

##
#### ResturentControllerApi

All URIs are relative to *https://localhost:8090*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getResturentUsingGET**](ResturentControllerApi.md#getResturentUsingGET) | **GET** /resturent | getResturent

##
#### DistancesControllerApi

All URIs are relative to *https://localhost:8090*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getDistanceUsingGET**](DistancesControllerApi.md#getDistanceUsingGET) | **GET** /distance | getDistance
## Documentation for Models.
Restaurant Model class *https://github.com/COMP4381/Team19/blob/master/Restaurant.md*
Distance Model class *https://github.com/COMP4381/Team19/blob/master/DistanceModelClass.md*
User Model class *https://github.com/COMP4381/Team19/blob/master/UserModelClass.md*
## Author
###### abed alamleh.
###### Muayed Mafarjeh.
