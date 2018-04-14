# springclould with server config

# Start spring boot  
mvn clean spring-boot:run

# alias for pretty json  
alias json_pretty='python -mjson.tool'  

# test api with curl  
curl http://localhost:8888/application/default | json_pretty  

curl http://localhost:8888/app-service-2/default | json_pretty  

curl http://localhost:8888/s1app/default | json_pretty  
curl http://localhost:8888/s1app/dev | json_pretty  
curl http://localhost:8888/s1app/qa | json_pretty  

curl http://localhost:8888/s3app/perf | json_pretty  
curl http://localhost:8888/application/perf | json_pretty  
