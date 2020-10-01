FROM ubuntu:18.04
RUN apt update && apt install git default-jdk maven -y
WORKDIR /home/sampleTest
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
WORKDIR /home/sampleTest/boxfuse-sample-java-war-hello
RUN mvn package
RUN mkdir /home/war && cp ./target/hello-1.0.war /home/war/