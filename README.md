# zipkin-sleuth-demo
Sleuth is another tool from the Spring cloud family. It is used to generate the trace id, span id and add this information to the service calls in the headers and MDC, so that It can be used by tools like Zipkin and ELK etc. to store, index and process log files.

Step 1 : Build All Micro Services using  command : mvn clean install.

step 2: Run all Micro Service.

step 3: Run Zipking Jar (from project directory) using this command: java -jar zipkin-server-2.12.9-exec.jar

step 4: Open this URL in browser : http://localhost:9411

step 5: Call this endpoint from postman: http://localhost:8080/microservice1

step 6: check traceId , spanId and parentId in zipkin UI(localhost:9411)
