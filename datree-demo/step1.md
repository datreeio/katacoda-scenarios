[Datree](https://datree.io/) is a CLI solution that supports Kubernetes owners in their roles, by preventing developers from making errors in Kubernetes configurations that can cause clusters to fail in production. 

## Task

### 1. Install Datree

The following command will install the CLI bineries:
`curl https://get.datree.io | /bin/bash`{{execute}}

### 2. Open the Kubernetes manifest file

We also added a pre-configured Kuberenetes manifest file to test - you can open it to check it out:  
`.datree/k8s-demo.yaml`{{open}}

### 3. Run the first invocation

The following command will test the `k8s-demo` agaisnt 21 built-in rules to find common misconfigurations:
`datree test ~/.datree/k8s-demo.yaml`{{execute}}

In the terminal output you should something like that:
<pre>
![demo output](./assets/demo-output.png)
</pre>
