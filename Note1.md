# Aws EBS
* we can easily scale
* high availability
* There is general purpose ssds
* There is I/O optimized SSDs
* There is throughput optimized HDD (low cost)
    * used for throughput intensive workloads, Big Data
    * There is a cold HDD (cheap)
    * Hdd cannot be used for boot 
* There is provisionsed IOPS if the IOPS is more than 16000 go for provisioned IOPS
![image](https://github.com/ronitwilson/aws_developer-cert/assets/9934360/0a202e87-11b1-429c-9909-fbb67fddee32)

# Aws Api gateway
* Publish, Maintain and monitor and secure APIs
* supports **RESTful api's** optimized for stateless, serverless workloads
* **websocket API's **
* supports multiple endpoints and targets
* supports multiple versions like development, testing production etc
* It supports throttling, so you manage traffice with traffic spikes etc 

# Aws cli
* The aws cli in the backend has a **pagination** of 1000
* setting **pagination** helps to define the number of api calls it will make. though it may still show/display all the info in one page
    * meaning the backend of the cli logic will try to make calls after each 1000 objs to get the next set
* if the objs are too large can get **timeout**,  then we need to make pagination
    * which will mean the cli will make multiple api calls to the backend
* Example aws s3api list-objects --bucket my-bucket --page-seize 10
    * other option is to use the --max-items

# Aws Parameter store
* store confidential information
* can store in plain text or encrypted
* can be integrated with aws services like ec2 lambda codebuild codepipeline etcc

# Ec2 image builder
### Ec2 builder workflow
![image](https://github.com/ronitwilson/aws_developer-cert/assets/9934360/769d1d02-9255-47b6-924a-cf7d4967682f)
