Create Application in Argocd

### Declarative Setup
Argo CD applications, projects and settings can be defined declaratively using Kubernetes manifests. 
These can be updated using kubectl apply, without needing to touch the argocd command-line tool.
![Screenshot from 2023-06-03 14-10-37](https://github.com/aadilraza339/udemy-app-definition/assets/47937273/a2f40e65-0e42-49c6-80b0-1604910d1311)
### Create Argo Cd Application.
Define an Argo Cd application declaratively using Yaml. </br>
You get over view how to create application using Yaml here is [link](https://github.com/aadilraza339/udemy-app-definition/blob/main/application.yaml)

Run this command on termial to crate application in Argo CD
```
kubectl apply -f application.yaml 

```
Output: </br>
![image](https://github.com/aadilraza339/udemy-app-definition/assets/47937273/345b2e7a-4ae0-465a-b17f-8f6e5528f58a)

### We also can create application using Argocd UI
![image](https://github.com/aadilraza339/udemy-app-definition/assets/47937273/02af4583-aca5-4cd9-b1d8-4ed8350a0542)
Please complete the required fields to create the application.

### Create application using CLI
Command:
```
argocd app create demo-app-for-testin --repo https://github.com/aadilraza339/udemy-coruse.git --path guestbook --dest-namespace default --dest-server https://kubernetes.default.svc --directory-recurse

```
Output: </br>
![image](https://github.com/aadilraza339/udemy-app-definition/assets/47937273/3d0330e7-2488-4f13-b07e-38a870e1b37a)

