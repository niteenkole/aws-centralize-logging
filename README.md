# aws-centralize-logging
Enterprise Environment AWS cloudtrail, config, vpcflow centralize logging in multi account setup

# Requirement
In enterprise environment like bank,finance etc where you have huge numbers of AWS accounts  having centralize logging becomes key requirement.


Example: 
   
Collecting all cloudtrail,config logs from all accounts in central location and then say pushing to splunk security (SOC requirement).

Automating centralize log collection also play key component to make operation process easy.

Collecting VPC flow logs from all accounts and pushing to central location then push to required logging tool like splunk.

Centralizing application logs and then pushing to required logging tool like splunk.

# Basically we have 3 parts here.
# 1. Cloudtrail and config logs.
# 2. Centralize vpcflowlogs.
# 3. Centralize Application logs.

# 1. Cloudtrail and config logs.
One method is to use centrally cloudtrail and config logs collected using AWS control tower method in central s3.
From there we can use say splunk pull method (ADDON) 

Steps:
