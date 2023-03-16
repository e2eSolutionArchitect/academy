# Integrate Tableau with Amazon Redshift

![image](https://user-images.githubusercontent.com/62712515/225402658-b862948d-20e2-480d-8ae5-215667e95daa.png)

## Frequent Issues and Fix:

An error occurred while communicating with the Amazon Redshift data source 'Untitled Data Source'
Unable to connect to the server. Check that the server is running and that you have access privileges to the requested database.
Error Code: 298A3F01
[Amazon][Amazon Redshift] (10) Error occurred while trying to connect: [SQLState 08S01] connection to server at "e2esa-rs-cluster-01.dfsdfsdf234werw.us-east-1.redshift.amazonaws.com" (48.51.123.28), port 5439 failed: Connection timed out (0x0000274C/10060)
	Is the server running on that host and accepting TCP/IP connections?

Unable to connect to the Amazon Redshift server "e2esa-rs-cluster-01.dfsdfsdf234werw.us-east-1.redshift.amazonaws.com". Check that the server is running and that you have access privileges to the requested database.

### Fix
- Check if your amazon redshift cluster is publicly accessible. Please check the steps in the video tutorial 
- Check the security group attached to the cluster has the inbound rule which allows internet traffic
