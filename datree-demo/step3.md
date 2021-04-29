
The following command will test the `k8s-demo` agaisnt 21 built-in rules to find common misconfigurations:
`datree test ~/.datree/k8s-demo.yaml`{{execute}}

In the terminal output you should something like that:

![demo output](./assets/demo-output.png)

### 1. fix label misconfiguration:

Replace the invalid owner label value `--` (owner: --) with a proper string:  
<pre class="file" data-filename=".datree/k8s-demo.yaml" data-target="insert"  data-marker="--">backend-team</pre>

### 2. fix image tag misconfiguration:

Replace `latest` (nginx:latest) with an fixed version:  
<pre class="file" data-filename=".datree/k8s-demo.yaml" data-target="insert"  data-marker="nginx:latest">nginx:1.4.6</pre>
