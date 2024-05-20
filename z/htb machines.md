Name= responder
level = very easy


nmap -p- --min-rate 1000 -sV 10.129.76.153


if we find a users creds that has access to windows remote management or WInRM than we can potentially get a reverse shell 
