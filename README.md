# MyNmapShScript

[ ![Relwarc17](https://www.hackthebox.eu/badge/image/278078)](https://www.hackthebox.eu/home/users/profile/278078)

This is my Nmap sh script that I use every time.

# Using:
```
sh nmap.sh ip_here
```

# Example output:
```
ubuntu@ubuntu:pts/1-> /home > ubuntu > ctf (0)
> sh nmap.sh 192.168.0.1
Starting Nmap 7.91 ( https://nmap.org ) at 2021-07-15 13:52 UTC
Nmap scan report for 192.168.0.1
Host is up (0.00051s latency).

PORT     STATE SERVICE VERSION
23/tcp   open  telnet
| fingerprint-strings:
|   GenericLines:
|     password:
|     Login incorrect. Try again.
|     password:
|     Login incorrect. Try again.
|     password:
|   GetRequest:
|     HTTP/1.0
|     password:
|     Login incorrect. Try again.
|     password:
|     Login incorrect. Try again.
|     password:
|   NCP:
|     DmdT^@^@^@
|     ^@^@^@^A^@^@^@^@^@
|   NULL:
|_    password:
80/tcp   open  http
| fingerprint-strings:
|   GetRequest:
|     HTTP/1.1 200 OK
|     Content-Type: text/html; charset=utf-8
|     Content-Length: 63635
|     Set-Cookie: JSESSIONID=deleted; Expires=Thu, 01 Jan 1970 00:00:01 GMT; Path=/; HttpOnly
|     Connection: keep-alive
|     <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
|     "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
|     <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
|     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
|     <head>
|     <link rel="shortcut icon" type="image/x-icon" href="../img/favicon.ico"/>
|     <link rel="stylesheet" href="../css/main.css"/>
|     <link rel="stylesheet" href="../css/login.css"/>
|     <link rel="stylesheet" href="../css/jquery.tpInput.css"/>
|     <script src="../js/jquery-1.8.3.min.js" type="text/javascript"></script>
|     <script src="../js/oid_str.js" type="text/javascript"></script>
|     <script src="../js/lib
|   HTTPOptions, RTSPRequest:
|     HTTP/1.1 405 Method Not Allowed
|     Content-Type: text/html; charset=utf-8
|     Content-Length: 124
|     Set-Cookie: JSESSIONID=deleted; Expires=Thu, 01 Jan 1970 00:00:01 GMT; Path=/; HttpOnly
|     Connection: close
|_    <html><head><title>405 Method Not Allowed</title></head><body><center><h1>405 Method Not Allowed</h1></center></body></html>
|_http-title: Site doesn't have a title (text/html; charset=utf-8).
1900/tcp open  upnp    Portable SDK for UPnP devices 1.6.19 (Linux 3.10.14; UPnP 1.0)
7547/tcp open  http    Remote access
|_http-server-header: tr069 http server
|_http-title: Site doesn't have a title (text/plain; charset=ISO-8859-1).
2 services unrecognized despite returning data. If you know the service/version, please submit the following fingerprints at https://nmap.org/cgi-bin/submit.cgi?new-service :
//Some fingerprints
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel:3.10.14
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .

```

