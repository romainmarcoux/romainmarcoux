English version [below](https://github.com/romainmarcoux#en-infos)

# [FR] Infos
Ce GitHub mets à disposition des agrégations de listes d'**adresses IP, domaines et hash malveillants** prêts à être implémentées sur vos systèmes de sécurité : pare-feux (notamment FortiGate), serveurs Web, WAF, proxy ...
- À bloquer en **entrée** (WAN > LAN) :
  * [malicious-ip](https://github.com/romainmarcoux/malicious-ip) : agrégation d'adresses IP malveillantes (scanners, bruteforce ...)
    * Statistiques mises à jour quotidiennement (~500k IP) : [historiques](https://github.com/romainmarcoux/malicious-ip/blob/main/statistics/historical_statistics.md), par [pays](https://github.com/romainmarcoux/malicious-ip/blob/main/statistics/country_statistics.md), par [AS](https://github.com/romainmarcoux/malicious-ip/blob/main/statistics/as_statistics.md)
    * Mon [tutorial](https://www.linkedin.com/posts/romainmarcoux_bloquer-des-ip-de-listes-externes-sur-fortigate-activity-7112413515725852673-KD4q) d'implémentation sur pare-feu Fortinet FortiGate ([liens](https://github.com/romainmarcoux/malicious-ip#implementation) pour les autres pare-feux)
    * Mon [post](https://www.linkedin.com/posts/romainmarcoux_fortinet-cybersaezcuritaez-saezcuritaezinformatique-activity-7152937338313089024-XrLA) avec des statistiques montrant la pertinence vis à vis de l'ISDB Malicious Server des FortiGate
    * Mon [tutorial](https://www.linkedin.com/posts/romainmarcoux_webinar-sekio-fortinet-tips-fortigate-activity-7109827284517146627-WK_4) (à partir de la page 18) pour filtrer le VPN SSL FortiGate dans les règles de filtrage afin de pouvoir le protéger de ces IP malveillantes 
- À bloquer en **sortie** (LAN > WAN) :
  * [malicious-outgoing-ip](https://github.com/romainmarcoux/malicious-outgoing-ip) : agrégation d'adresses IP malveillantes (phishing, malware, C2 ...)
  * [malicious-domains](https://github.com/romainmarcoux/malicious-domains) : agrégation de domaines malveillants (phishing / hameçonnage, malware ...)
    * Implémentable sur les pare-feux FortiGate via le DNS Filter : voir [README](https://github.com/romainmarcoux/malicious-domains)
  * [malicious-hash](https://github.com/romainmarcoux/malicious-hash) : agrégation d'empreintes (hash) de fichiers malveillants
    * Implémentable sur les pare-feux FortiGate via les profils AntiVirus (voir [README](https://github.com/romainmarcoux/malicious-hash))

![Schema](https://sekio.fr/img/schema.jpg 'schema')

Les éléments sont ordonnés en fonction du nombre de sources dans lesquelles ils apparaissent : des plus malveillants aux moins malveillants. 

**Lire attentivement** le README de chaque agrégation : fréquence de mises à jour, nombre d'éléments, implémentation, liens des fichiers, liste des sources ...

N'hésitez pas à vous connecter à mon [profil](https://linkedin.com/in/romainmarcoux/) LinkedIn et m'envoyer un message pour :
- me remercier et m'encourager 😉
- que je vous prévienne des évolutions et des nouveaux segments à ajouter dans vos systèmes
- me prévenir d'erreurs, problèmes, faux positifs ou d'IP / entrées DNS malveillantes qui seraient absentes de mes agrégations
- me solliciter pour bénéficier de mon expertise en cybersécurité (audit, conseil, intégration) que je propose en tant que __freelance__ à des **clients finaux** et en sous-traitance à des **partenaires** en manque de ressources ou d'expertise. Plus d'infos sur mon [profil](https://linkedin.com/in/romainmarcoux/) LinkedIn. 

# To support me

[![BuyMeACoffee](https://raw.githubusercontent.com/romainmarcoux/romainmarcoux/main/img/buymeacoffee.png 'BuyMeACoffee')](https://buymeacoffee.com/romainmarcoux)
[![Paypal](https://www.paypalobjects.com/en_US/FR/i/btn/btn_donateCC_LG.gif 'Paypal')](https://www.paypal.com/donate/?hosted_button_id=TNPNMMBFVVL8E)

# [EN] Infos

This GitHub provides aggregations of lists of **IP addresses, domains and malicious hashes** ready to be implemented on your security systems: firewalls (notably FortiGate), web servers, WAF, proxy, etc.
- To be blocked at **input** (WAN > LAN):
  * [malicious-ip](https://github.com/romainmarcoux/malicious-ip) : aggregation of malicious IP addresses (scanners, bruteforce, etc.) to be blocked at **input** (WAN > LAN)
- To block on **output** (LAN > WAN):
  * [malicious-outgoing-ip](https://github.com/romainmarcoux/malicious-outgoing-ip) : aggregation of malicious outgoing IP addresses (phishing, malware, C2 ...)  to be blocked at **output** (LAN > WAN)
  * [malicious-domains](https://github.com/romainmarcoux/malicious-domains) : aggregation of malicious domains (phishing / phishing, malware, etc.)
  * [malicious-hash](https://github.com/romainmarcoux/malicious-hash) : aggregation of hashes of malicious files (on FortiGate firewalls, can be implemented in AntiVirus profiles)

The items are ordered by the number of sources they appear in: from most malicious to least malicious.

**Read carefully** the README of each aggregation: frequency of updates, number of elements, implementation, file links, list of sources...

Feel free to connect to my LinkedIn [profile](https://linkedin.com/in/romainmarcoux/) and send me a message to:
- thank me and encourage me 😉
- that I notify you of developments and new segments to be added to your systems
- warn me of errors, problems, false positives or malicious IP / DNS entries that are missing from my aggregations
- ask me to benefit from my expertise in cybersecurity (audit, consulting, integration) which I offer as a __freelance__ to **end clients** and as a subcontractor to **partners** lacking resources or expertise. More info on my LinkedIn [profile](https://linkedin.com/in/romainmarcoux/).
