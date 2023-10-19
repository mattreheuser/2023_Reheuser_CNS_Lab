# 7330: Computer and Network Security Homework 6
## Matthew Reheuser  
#### 2023.10.18 <p>&nbsp;</p>

### - Splunk training course   
I took the Splunk training course on getting data into Splunk. This course helped closed a lot of the gaps I had in my mind about how the logs were getting into Splunk. There are four segments to get data into the pipeline. Starting with input, then the data is parsed, then indexed, then available for searching.  

Data input types are 
files and directories
network events
scripted outputs
linux and windows sources
HTTP(s) Protocl
Metrics

There are uboyt types and meta data
source types are very importatnt 

### - Splunk course certificate

### - Windows Event ID 

The Windows event ID I blacklisted from our splunk was 4624. 4624 is the event ID thaty gets passed when there is a successful login. The reason we choose to exclude that ID was because we though that information by itself was something that could produce a lot of logs while not adding much functionality for our team.  

### - Input.conf
The input.conf file is located within the etc/system of the SplunkUniversalForwarder. The etc folder is used to store system configuration files which makes sense for having the input configuration file in there. 
![File system](./pictures/fileStructure.png)  




