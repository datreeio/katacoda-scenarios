
### 1. Fix label misconfiguration:

Replace the invalid owner label value `--` (owner: --) with a proper string:  
<pre class="file" data-filename=".datree/k8s-demo.yaml" data-target="insert"  data-marker="--">backend-team</pre>

### 2. Fix image tag misconfiguration:

Replace `latest` (nginx:latest) with an fixed version:  
<pre class="file" data-filename=".datree/k8s-demo.yaml" data-target="insert"  data-marker="nginx:latest">nginx:1.4.6</pre>
