# spring-boot-with-cloudwatch-metrics
A spring-boot REST service that uses the micrometer library to send metrics to Cloudwatch

## Instructions
- launch EC2 instance using the following AWS-provided role: ```arn:aws:iam::832430016211:role/CloudWatchAgentServerRole```
- clone repo
- update application.properties with your AWS region
- mvn spring-boot:run
- browse Cloudwatch->Metrics

## TODO
(only capture the following metrics)
- (Tomcat) thread pool max & busy connections
- JVM heap size (with graph showing garbage collection)
- Database connection pool - free connections

## Complete
- Create simple REST service
- Push to my Git repository
- Install Java 1.8
- SCP Maven
- Add micrometer dependencies to poms.xml
- Install maven from zip and add to path

## Resources
https://dzone.com/articles/spring-boot-metrics-with-micrometer-and-aws-cloudw
$ scp -i my-blz-ley.pem /local/path/to/file/maven.tar.gz ec2-user@100.1.2.3  

Tomcat concurrency
https://www.e4developer.com/2018/03/30/introduction-to-concurrency-in-spring-boot/
