---
title: Verify node-exporter Chart Installation
description: This tutorial explains how to verify that node-exporter chart installed successfully
---


Once the helm chart installation done you need to verify all the pods and services are up and running.

Execute below command to check status of pods and services: 

### Check the pod status


```execute
kubectl get pods --namespace monitoring
```

You will see similar to this output:

```

```

It may take few minutes to change the `STATUS` from `ContainerCreating` to `Running`. 

```output


```

Once the `node-exporter` PODs are up and running , and `READY` states are `1/1`, your node-exporter is ready to use.

### Check all the Kubernetes resources status

You can run the following command to know status of all the deployed resources inside the namespace `node-exporter`


```execute
kubectl get all --namespace monitoring
```

All the deployment and service status should be Running.

```


```
