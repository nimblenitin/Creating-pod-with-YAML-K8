# Creating-pod-with-YAML-K8
Simple example to create Pod in Declarative method with YAML

##Steps followed-
*As Root*
```

1. Create the YAML file
vim podByDeclarative.yaml 

Type the YAML script-
apiVersion: v1
kind: Pod
metadata:
  name: declarative-pod
spec:
  containers:
    - name: mycontainer
      image: nginx
      ports:
      - containerPort: 80
      
2. Create the Pod-
kubectl apply -f podByDeclarative.yaml
 
3. View the Pod created:
kubectl get pods -o wide
 
 ```

