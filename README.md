# Analisi LOG

L'obiettivo di questo laboratorio è l'analisi di un LOG.

Tools utilizzati:
- Cyberchef
- Abuseipdb
- Virustotal
- DNSlytics
- OTXAlienvault
- Google Dorks


LOG proveninte dall'IPS:

***IPS BLOCK***
<185>Mar 27 16:58:32 172.1.8.22 <185>logver=600050268 timestamp=3285324711 tz="UTC+1:00" devname="IPSEXT" date=2020-03-27 time=16:58:31 logid="0419016384" type="utm" subtype="ips" eventtype="signature" level="alert" eventtime=3285324711 severity="medium" srcip=36.73.190.32 srccountry="Indonesia" dstip=172.2.193.1 action="detected" service="HTTPS" policyid=3125 srcport=51374 dstport=443 hostname="www.vulnerability.com" url="/aboutus/whoami.php?sVirtualURL=" profile="ips" ref="http://www.fortinet.com/ids/VID17702" incidentserialno=13473132," attackcontextid="1/2" attackcontext="PFBBVFRFUk5TPiA8c2NyaXB0OzxzY3JpcHQ7c2NyaXB0PjtzY3JpcHQ+PC9QQVRURVJOUz4KPFVSST4gR0VUIC9hYm91dHVzL3dob2FtaS5waHA/c1ZpcnR1YWxVUkw9PSI+PHNjcmlwdCUyMD5hbGVydChTdHJpbmcuZnJvbUNoYXJDb2RlKDg4LDgzLDgzKSk8L3NjcmlwdD4maUlERGFsUG9ydGFsZT0maUlETGluaz0tMSBIVFRQLzEuMTwvVVJJPgo8SEVBREVSPiBBY2NlcHQ6IFRleHQvSHRtbCxBcHBsaWNhdGlvbi9YaHRtbCBYbWwsQXBwbGljYXRpb24vWG1sO1E9MC45LCovKjtRPTAuOApDb25uZWN0aW9uOiBrZWVwLWFsaXZlClVzZXItQWdlbnQ6IE1vemlsbGEvNS4wIChXaW5kb3dzIE5UIDEwLjA7IFdPVzY0OyBSdjo1MC4wKSBHZWNrby8yMDEwMDEwMSBGaXJlZm94LzUwLjAKQWNjZXB0LUxhbmd1YWdlOiBlbi11cyxlbjtxPTAuNQpBY2NlcHQtRW5jb2Rpbmc6IGd6aXAKSG9zdDogd3d3LnZ1bG5lcmFiaWxpdHkuY29tCjwvSEVBREVSPgo8Qk9EWT4gPC9CT0RZPg=="

-- Inizio dell'analisi --

Utilizzo il tool Cyberchef per decifrare la parte di testo cifrata:
Per ottenere il testo in chiaro utilizzo la funzione "From Base 64"
Da questo log, proveniente dall’ips, è stato riscontrato che l’attaccante sta verificando se la pagina “whoami” del sito è vulnerabile ad un attacco XSS (Cross-Site Scripting):


<img width="1274" alt="cyberchef" src="https://github.com/user-attachments/assets/ca52658b-507b-4c5c-a524-3833b6eaf744">





