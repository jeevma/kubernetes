# Kubernetes kubectl Commands

## Overview

This document provides a list of commonly used `kubectl` commands for managing Kubernetes clusters.

## Installation

Before using `kubectl`, you need to install the Kubernetes command-line tool. Instructions can be found [here](https://kubernetes.io/docs/tasks/tools/install-kubectl/).

## Common Commands

**Get cluster information:**
```  kubectl cluster-info```

**List all pods in the current namespace**
```kubectl get pods```

**List all pods in a specific namespace**
```kubectl get pods -n <namespace>```

**Describe a pod**
```kubectl describe pod <pod_name>```

**Get detailed information about nodes**
```kubectl get nodes```

**Deploy an application from a YAML file**
```kubectl apply -f <path_to_yaml_file>```

**Scale a deployment**
```kubectl scale --replicas=<replica_count> deployment/<deployment_name>```

**Delete a pod**
```kubectl delete pod <pod_name>```

**Execute a command inside a pod**
```kubectl exec -it <pod_name> -- <command>```

**Get logs from a pod**
```kubectl logs <pod_name>```

**Port forwarding to a pod**
```kubectl port-forward <pod_name> <local_port>:<remote_port>```

**Create a secret from literal values**
```kubectl create secret generic <secret_name> --from-literal=<key>=<value>```

**Get a list of all available resources**
```kubectl api-resources```

**Create a deployment**
```kubectl create deployment <deployment_name> --image=<image_name>```

**Expose a deployment as a service**
```kubectl expose deployment <deployment_name> --port=<port_number> --type=<service_type>```

**Delete a deployment**
```kubectl delete deployment <deployment_name>```

**Scale a deployment**
```kubectl scale --replicas=<replica_count> deployment/<deployment_name>```

**Get the status of a deployment**
```kubectl rollout status deployment/<deployment_name>```

**Rollback a deployment to a previous revision**
```kubectl rollout undo deployment/<deployment_name>```

**Create a namespace**
```kubectl create namespace <namespace_name>```

**Delete a namespace**
```kubectl delete namespace <namespace_name>```

**Set the current context**
```kubectl config use-context <context_name>```

**Get a list of contexts**
```kubectl config get-contexts```

**Switch to a different namespace**
```kubectl config set-context --current --namespace=<namespace_name>```
