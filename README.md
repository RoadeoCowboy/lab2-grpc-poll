# lab2-grpc-poll
This is the GRPC lab2 for CMPE273

How to Run:
1. Login to EC2 Instance
2. $ ssh sjsu
3. $ cd protobuf/java/grpc-java-v1
4. $ ./gradlew install
5. $ ./gradlew :grpc-examples:pollServer
6. On seperate terminal
7. $ cd protobuf/java/grpc-java-v1 
8. $ ./gradlew :grpc-examples:pollClient
9. Expect output: Client $ INFO: Created a new poll with id = 1 
    Server: INFO: moderator Id is: 1

How to modify source files:
1. $ cd protobuf/java/grpc-java-v1/examples/src/main/java/edu/sjsu/cmpe273/lab2
2. $ nano pollServer.java
3. $ nano pollClient.java

If nothing works: $ gradle clean

Setup:
1. Create own path for source files.
2. ie: mkdir ../../grpc-java-v1/examples/src/main/java/edu/sjsu/cmpe273/lab2
3. Create proto file. $ ~/protobuf/java/grpc-java-v1/examples/src/main/proto/poll.proto
4. Modified build.gradle $ ~/protobuf/java/grpc-java-v1/examples/build.gradle
5. Added tasks pollServer and pollClient (These are java classes that need to be implemented, case-sensitive)

Follow additional readme instructions on how to build in the grpc-java-v1 folder.

