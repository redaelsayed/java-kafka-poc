# java-kafka-poc

- in a telecom company "Orange" we have a db with a table called "Customer" contains 1000,000 customer data 
    - name : String
    - phone : String
    - balance : float
- and we need to send a message to all these customers with format "Hello [name] you got 2X of your balance . you current balance is 2*[balance]"


- assumptions :
  - our database is mysql or postgres (choose your faivrout ) 
  - table strcuter 
      name :String
      phone:String
      balance:float
  - We have sms gateway to send the messages ( for now we will just write these massges to file(s))
  

Request:
 - buils a java program using Kafka to read the 1M users from db in batches 
 - prepare a message for each user and write this message to kafka topic 
 - build a java consumer(s) to read these messages and write them to file(s)
 
 
