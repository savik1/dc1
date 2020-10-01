FROM maven:3.6.3
RUN uname -a
RUN apt-get update && apt-get install -y git
WORKDIR /home/sampleTest
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
WORKDIR /home/sampleTest/boxfuse-sample-java-war-hello
RUN mvn package
RUN mkdir /home/war && cp ./target/hello-1.0.war /home/war/