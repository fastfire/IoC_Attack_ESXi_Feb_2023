# IoC_Attack_ESXi_Feb_2023
Collection of IoCs available and related to attacks on ESXi infrastructures that occurred as of Friday February 3, 2023.

**News**

Here are some references regarding the attack:

https://www.cert.ssi.gouv.fr/alerte/CERTFR-2023-ALE-015/

https://blog.ovhcloud.com/ransomware-targeting-vmware-esxi/

https://www.bleepingcomputer.com/news/security/massive-esxiargs-ransomware-attack-targets-vmware-esxi-servers-worldwide/

**Recover you systems**

Some really useful information to proceed with the recovery of compromised servers

https://enes.dev/

Script that extracts a list of some compromised instances (not all but probably those compromised by the Threat Actor himself). The script also extracts the list of Bitcoin Wallets indicated to pay the ransom, useful for some matches of any Wallets already used elsewhere:

**Payments tracking**

https://gist.github.com/achillean/33fe43afc36208a595e75200cb7abe97

**Compromised surface**
it is possible to get a good idea of the compromised surface using these queries within Shodan and Censys:

Shodan: https://beta.shodan.io/search?query=html%3A%22We+hacked+your+company+successfully%22+title%3A%22How+to+Restore+Your+Files%22

Censys: https://search.censys.io/search?resource=hosts&sort=RELEVANCE&per_page=25&virtual_hosts=EXCLUDE&q=services.http.response.html_title%3A%22How+to+Restore+Your+Files%22
