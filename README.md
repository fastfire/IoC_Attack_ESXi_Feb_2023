# IoC_Attack_ESXi_Feb_2023
Collection of IoCs available and related to attacks on ESXi infrastructures that occurred as of Friday February 3, 2023.

**News**

Here are some references regarding the attack:

https://www.cert.ssi.gouv.fr/alerte/CERTFR-2023-ALE-015/

https://blog.ovhcloud.com/ransomware-targeting-vmware-esxi/

https://www.bleepingcomputer.com/news/security/massive-esxiargs-ransomware-attack-targets-vmware-esxi-servers-worldwide/

**Recover your systems**

Some really useful information to proceed with the recovery of compromised servers

https://enes.dev/

**Payments tracking**

Script that extracts a list of some compromised instances (not all but probably those compromised by the Threat Actor himself). The script also extracts the list of Bitcoin Wallets indicated to pay the ransom, useful for some matches of any Wallets already used elsewhere:

https://gist.github.com/achillean/33fe43afc36208a595e75200cb7abe97

**Compromised surface**

It is possible to get a good idea of the compromised surface using these queries within Shodan and Censys:

Shodan (837 compromised hosts on February 6rd): https://beta.shodan.io/search?query=html%3A%22We+hacked+your+company+successfully%22+title%3A%22How+to+Restore+Your+Files%22

Censys (3276 compromised hosts on February 6rd): https://search.censys.io/search?resource=hosts&sort=RELEVANCE&per_page=25&virtual_hosts=EXCLUDE&q=services.http.response.html_title%3A%22How+to+Restore+Your+Files%22

**Encryption script**

At the link https://www.bleepingcomputer.com/forums/t/782193/esxi-ransomware-help-and-support-topic-esxiargs-args-extension/page-14#entry5470686 the scripts used by the Threat Actor to encrypt the systems were shared: 

Full script https://pastebin.com/y6wS2BXh

Script + encrypt binary https://we.tl/t-QMYhnF5evE
