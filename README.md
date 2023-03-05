# Kuberntes Microservice Application

## How to run it?

Execute the following command

```sh
kubectl create -f .
```

Or run the following scripts

```sh
Windows: deployment-script-windows.bat
Unix: deployment-script-unix.sh
```

## How to access the application?

Check the NodePort created by executing the command, you will notice a NodePort Service created with a specific port from 30000-32767

```sh
kubectl get services
```

Access the application by concatenating the IP of the node (or localhost if running a local instance)

```sh
[IP_ADDRESS / localhost]:[NODEPORT_PORT]
```

## Architecture Diagram

![Microservice Application](/application_diagram.png "Microservice Application")