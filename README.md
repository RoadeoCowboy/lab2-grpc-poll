# lab2-grpc-poll
This is the GRPC lab2 for CMPE273

How to Run:
1.) Login to EC2 Instance
2.) $ ssh sjsu
3.) $ cd protobuf/java/grpc-java-v1
4.) $ ./gradlew install
5.) $ ./gradlew :grpc-examples:pollServer
6.) On seperate terminal
7.) $ cd protobuf/java/grpc-java-v1 
8.) $ ./gradlew :grpc-examples:pollClient
9.) Expect output: Client $ INFO: Created a new poll with id = 1 
    Server: INFO: moderator Id is: 1

How to modify source files:
1.) $ cd protobuf/java/grpc-java-v1/examples/src/main/java/edu/sjsu/cmpe273/lab2
2.) $ nano pollServer.java
3.) $ nano pollClient.java
