# HyperText Transfer Protocol (HTTP)

### **To get the flag, start the above exercise, then use cURL to download the file returned by '/download.php' in the server shown above.**

```bash
curl -s -O http://134.122.105.9:31551/download.php
```

We downloaded our file. Let’s check it.

```bash
(root💀kali)-[~/Downloads/123]
└─# ls    
download.php
```

File seems fine. Let’s open it:

<pre class="language-bash"><code class="lang-bash"><strong>(root💀kali)-[~/Downloads/123]
</strong>└─# cat download.php
</code></pre>

<figure><img src="../../../../../.gitbook/assets/Untitled.png" alt=""><figcaption></figcaption></figure>
