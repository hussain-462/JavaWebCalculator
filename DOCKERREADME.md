 Java Web Calculator App — Docker Deployment

 Description
This is a Java web-based calculator application containerized using Docker. The app is packaged as a `.war` file and deployed inside a Docker container running Tomcat with Java 17.

 What I Did
- Built the project using Maven to generate the `.war` file.  
- Created a Dockerfile to build a custom Docker image including the `.war` file.  
- Built and ran the Docker container hosting the app on port 8080.

 Tools & Technologies
- Docker  
- Maven  
- Java 17  
- Tomcat 9  

 How to Run

1. Clone the repository:  
  
   git clone https://github.com/username/java-web-calculator.git
   cd java-web-calculator
Build the project with Maven:
mvn compile
mvn verify
mvn test
mvn package
Build the Docker image:
docker build -t java-web-calculator .
Run the Docker container:
docker run -d -p 8080:8080 java-web-calculator
Access the application by opening your browser to:

http://<EC2-instance-public-IP>:8080/<war-file-name>/
Replace <EC2-instance-public-IP> with your server’s IP and <war-file-name> with the name of the .war file deployed.
