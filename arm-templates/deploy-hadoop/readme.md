# Deploy Hadoop Cluster using Ambari

Clicking on the **Deploy to Azure** button below will deploy the following

* Single Ambari Server VM
* Multiple Hadoop Server VMs

Once the Infrastructure is deployed, the following actions will take place on the Ambari Server VM

* DNS will be installed and the provided Domain Name in the ARM Template will be registered
* The Ambari Server repo is downloaded and installed on the Ambari VM.
* All deployed Servers will have their **/etc/hosts** file modified to contain the IP Address, FQDN, and Hostname of all deployed Servers
* iptables and Transparent Huge Pages is disabled on all Servers


<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https://raw.githubusercontent.com/martinthiele/deploy-ambari-centos/master/arm-templates/deploy-hadoop/vs-project/deploy-hadoop/Templates/azuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

The Ambari is external accessible using the deployed public IP Address on ports 22 and 8080


## Related Articles

