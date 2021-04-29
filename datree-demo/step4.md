
Check out line #7 in `k8s-demo` file.

❌ The `owner` value is an invalid label value (--) so it will not get accepted when will try to deploy this file.

### Let's fix label misconfiguration:
Replace the invalid owner label value `--` (owner: --) with a proper string:  
➡️ <pre class="file" data-filename=".datree/k8s-demo.yaml" data-target="insert"  data-marker="--">backend-team</pre>
