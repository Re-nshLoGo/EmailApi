# EmailApi
This is an Email API built using Spring Boot and adding javax.mail dependency.
The API allows users to send emails from one user to another user. Users can send emails with Attachments and without Attachments.
### Requirments -
 * IntelliJIDEA
 * Serverport: 8080 (use: localhost:8080)
 * Java version: 17
 * Everything is present in the pom.xml (no need to download any library)
  ### Steps to run program -
 * Download the source code and import in intellijIDEA.
 * Go to localhost:8080/ 
 * Type endpoints in postman and insert values
 ## send email - 
     For create session use a valid email and app password.
 ### There is one model for EmailTemplate which has the following attributes -
 * From (sender email address)
 * To (Receiver email address)
 * Subject
 * Message
 ### For sending Emails with attachments use form-data in the Body that will be in key-value pair -
 1) - 1st parameter will be type of a file and in value choose a file to be sent.
 2) - 2nd parameter will be the text type that contains attributes of EmailTemplate in JSON format.
 ### Note
* You can change server port by setting properties in application.properties file i.e.

        server.port=8081
 
 
