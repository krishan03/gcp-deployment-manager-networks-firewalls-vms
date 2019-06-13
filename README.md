# gcp-deployment-manager-networks-firewalls-vms
Network deployment on Google cloud using Deployment Manger

This repository will deploy 2 networks with firewall rules and compute engine instances, as shown in the diagram below:

![alt text](https://github.com/krishan03/gcp-deployment-manager-networks-firewalls-vms/blob/master/network.png)

To use this, make sure tha you have a valid GCP account and the GCP project with billing enabled. Alos, make sure that Deployment Manager API is enabled in your GCP project.
Activate the cloud shell and create the folder and copy the git repository. From inside the cloned folder, run the below command to create the resources as shown in the diagram:

```
gcloud deployment-manager deployments create gcpnetwork --config=config.yaml
```

where gcpnetwork is the name of the deployment.

To delete the deployment, run the below command from the cloned folder:

```
gcloud deployment-manager deployments delete gcpnetwork
```


Happy Coding!!!
