# sysPass
[sysPass](https://github.com/nuxsmin/sysPass) is a web application that provides a password management in a secure and collaborative way.


# sysPass on Kubernetes
* To better group and manage the components of the solution it is recommended to create a dedicated namespace in the cluster:

```  
kubectl create namespace syspass
```

* Go to the folder that you have cloned the source code
* To create services and statefulsets, run the following command: 

```  
kubectl apply -n syspass -f syspass-mysql.yml -n syspass -f syspass-svc.yml -n syspass -f loadbalancer.yml
```
