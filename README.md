# Calico Helm Chart

I took AWS/EKS Calico Installation file that you can find here https://docs.aws.amazon.com/eks/latest/userguide/calico.html and split it into few files that make up the whole Helm Chart.

I have not worked on creating values.yaml file and templating it much, so if you have suggestions or time, feel free to update it. I just used the helm chart to test few things with automated Deployment. 


# Installation

Clone this repository

and then run

```
helm install . --name=calico --namespace=kube-system 
```
If you need to reference tiller, just add --tiller-namespace=NamespaceWhereTillerIsInstalled



# Notes

This helm chart is really straight forward, however feel free to fork it or make changes. I'll see to make updates to values files and start disecting the yaml infrastructure within the template. 
