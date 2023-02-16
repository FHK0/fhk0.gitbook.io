# HTTP Requests and Responses

### **What is the HTTP method used while intercepting the request? (case-sensitive)**

Answer: G\*\*

### **Send a GET request to the above server, and read the response headers to find the version of Apache running on the server, then submit it as the answer. (answer format: X.Y.ZZ)**

Let’s send cURL request and look for the response.

```bash
(root💀kali)-[~]
└─# curl -I http://161.35.169.248:31661/
```

The answer is in the server header.

<figure><img src="../../../../../.gitbook/assets/Untitled (3).png" alt=""><figcaption></figcaption></figure>
