# HTTP Headers

### The server above loads the flag after the page is loaded. Use the Network tab in the browser devtools to see what requests are made by the page, and find the request to the flag.

<figure><img src="../../../../../.gitbook/assets/Untitled (3) (1).png" alt=""><figcaption></figcaption></figure>

We spotted the flag request. Let’s send cURL request to get the flag.

```bash
(root💀kali)-[~]
└─# curl http://161.35.169.248:30047/flag_327a6c4304ad5938eaf0efb6cc3e53dc.txt
```

<figure><img src="../../../../../.gitbook/assets/Untitled 1 (2).png" alt=""><figcaption></figcaption></figure>
