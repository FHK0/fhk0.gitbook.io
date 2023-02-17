# POST

### Obtain a session cookie through a valid login, and then use the cookie with cURL to search for the flag through a JSON POST request to '/search.php’

<figure><img src="../../../../../.gitbook/assets/Untitled (1).png" alt=""><figcaption></figcaption></figure>

The cURL command we copied is:

```bash
curl 'http://178.62.24.63:32137/search.php' -X POST -H 'User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0' -H 'Accept: */*' -H 'Accept-Language: en-US,en;q=0.5' -H 'Accept-Encoding: gzip, deflate' -H 'Referer: http://178.62.24.63:32137/' -H 'Content-Type: application/json' -H 'Origin: http://178.62.24.63:32137' -H 'Connection: keep-alive' -H 'Cookie: PHPSESSID=t3jks0j77ncate6d7j0nvu9nn9' --data-raw '{"search":"Paris"}'
```

Let’s reshape our command with only necessary headers and search for flag:

```bash
curl -X POST -d '{"search":"flag"}' -H 'Content-Type: application/json' -H 'Cookie: PHPSESSID=t3jks0j77ncate6d7j0nvu9nn9' http://178.62.24.63:32137[/search.php](http://68.183.36.105:32270/search.php)
```

<figure><img src="../../../../../.gitbook/assets/Untitled 1 (2).png" alt=""><figcaption></figcaption></figure>
