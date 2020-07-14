# avi_on_azure

Ansible Scripts to Deploy AVI Controllers and AVi Service Engines on AZURE Cloud.
Ansible Scripts used to manage AVI Life Cycle ( creating Virtual Service,Pools,Cloud,Health Monitor,GSLB,etc...)

Basic Infrastructure 	Description
configController.yml	Perform Basic controller configuration
configCloud.yml	Create Cloud on Controller per vnet
avi_config_role.yml	 
configCluster.yml	From Controller cluster of 3 nodes
configClusterclouddetails.yml	Register cluster virtual IP to Azure
configAlertconfig.yml	Configure alerts
 	 
Application Profile	 
configApplicationprofilehttp.yml	Configure HTTP Application Profile
configApplicationprofilel4.yml	Configure L4 Application Profile
configDnsprofile.yml	Configure DNS Application Profile for GSLB
 	 
Persistence Profile	 
configClientippersistence.yml	Configure  Client IP Persistence under pool
 	 
Health Monitors	 
configHealthmonitor.yml	Configure HTTP Health Monitor
configHealthmonitortcp.yml	Configure TCP Health Monitor
 	 
Analytics	 
configAnalyticsprofile.yml	Configure Analytics Profile
configAlertsyslog.yml	Configure alerts to syslog server
 	 
SSL/TLS Certificates	 
configCsr.yml	Generate CSR and display Key
configUploadcert.yml	Upload certificate to Controller
 	 
SSL/TLS Profile	 
configSslprofile.yml	Configure SSL Profile
 	 
Service Engine Group	 
configSegroup.yml	Configure Service Engine Group
 	 
Pool	 
configPool.yml	Configure Pool using Server IP
configPoolscalset.yml	Configure Pool using Azure scale set
configPoolreplace.yml	Replace the existing pools with new pool members
 	 
Virtual Service	 
configVirtualservice.yml	Configure Virtual Service
 	 
GSLB	 
configGslbdnsvs.yml	Configure GSLB DNS vs
configGslbdomain.yml	Configure GSLB  Sub Domain
configGslbservice.yml	Configure GSLB Service Active Active
configGslbserviceactive_standby.yml	Configure GSLB Service Active Standby
configThirdpartyservice.yml	Configure GSLB Third Party Service 
 	 
WAF	 
configWafpolicy.yml	Configure Waf Policy
configWafprofile.yml	Configure Waf Profile
vs-1-waf-policy-patches.json	Attach rules to waf
