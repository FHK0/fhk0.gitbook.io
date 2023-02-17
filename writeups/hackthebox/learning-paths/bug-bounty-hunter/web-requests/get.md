# GET

### The exercise above seems to be broken, as it returns incorrect results. Use the browser devtools to see what is the request it is sending when we search, and use cURL to search for 'flag' and obtain the flag.

<figure><img src="../../../../../.gitbook/assets/Untitled (1) (1).png" alt=""><figcaption></figcaption></figure>

The cURL command we copied is:

```bash
curl 'http://68.183.35.199:30104/search.php?search=Leicester' -H 'User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0' -H 'Accept: */*' -H 'Accept-Language: en-US,en;q=0.5' -H 'Accept-Encoding: gzip, deflate' -H 'Referer: http://68.183.35.199:30104/' -H 'Authorization: Basic YWRtaW46YWRtaW4=' -H 'Connection: keep-alive'
```

In the command, I can see that there is a token that maintains my `admin:admin` login which is:

```bash
'Authorization: Basic YWRtaW46YWRtaW4='
```

Let’s send a simple cURL request to get the flag:

```bash
(root💀kali)-[~]
└─# curl -H 'Authorization: Basic YWRtaW46YWRtaW4=' http://68.183.35.199:30104/search.php?search=flag
```

<figure><img src="../../../../../.gitbook/assets/Untitled 1 (1).png" alt=""><figcaption></figcaption></figure>
