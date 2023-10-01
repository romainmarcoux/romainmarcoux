# [FR] Infos
Ce GitHub mets à disposition des agrégations d'**adresses IP, domaines et hash malveillants** prêts à être implémentées sur vos systèmes de sécurité : pare-feux (notamment FortiGate), serveurs Web, WAF, proxy ...
- À bloquer en **entrée** (WAN > LAN) :
  * [malicious-ip](https://github.com/romainmarcoux/malicious-ip) : agrégation d'adresses IP malveillantes (scanners, bruteforce ...)
    * Statistiques mises à jour quotidiennement :
      * [historiques](https://github.com/romainmarcoux/malicious-ip/blob/main/statistics/historical_statistics.md) : nombre de sources, d'IP, part présent dans 6 sources et 1 source, part commune avec l'ISDB Malicious Server des FortiGate
      * par [pays](https://github.com/romainmarcoux/malicious-ip/blob/main/statistics/country_statistics.md)
      * par [AS](https://github.com/romainmarcoux/malicious-ip/blob/main/statistics/as_statistics.md) (propriétaire de l'adresse IP)
    * Mon [tutorial](https://www.linkedin.com/posts/romainmarcoux_bloquer-des-ip-de-listes-externes-sur-fortigate-activity-7112413515725852673-KD4q) d'implémentation sur pare-feu Fortinet FortiGate ([liens](https://github.com/romainmarcoux/malicious-ip#implementation) pour les autres pare-feux)
    * Mon [post](https://www.linkedin.com/posts/romainmarcoux_fortinet-cybersaezcuritaez-saezcuritaezinformatique-activity-7152937338313089024-XrLA) avec des statistiques montrant la pertinence vis à vis de l'ISDB Malicious Server des FortiGate
    * Mon [tutorial](https://www.linkedin.com/posts/romainmarcoux_webinar-sekio-fortinet-tips-fortigate-activity-7109827284517146627-WK_4) (à partir de la page 18) pour filtrer le VPN SSL FortiGate dans les règles de filtrage afin de pouvoir le protéger de ces IP malveillantes 
- À bloquer en **sortie** (LAN > WAN) :
  * [malicious-outgoing-ip](https://github.com/romainmarcoux/malicious-outgoing-ip) : agrégation d'adresses IP malveillantes (phishing, malware, C2 ...)
    * Attention : encore en beta test jusqu'à août 2024
  *  [malicious-domains](https://github.com/romainmarcoux/malicious-domains) : agrégation de domaines malveillants (phishing / hameçonnage, malware ...)
    * Implémentable sur les pare-feux FortiGate via le DNS Filter : voir [README](https://github.com/romainmarcoux/malicious-domains)
    * Pour éviter les faux positifs, les domaines du top 1M des sites Web les plus visités ont été retirés.
  * [malicious-hash](https://github.com/romainmarcoux/malicious-hash) : agrégation d'empreintes (hash) de fichiers malveillants
    * Implémentable sur les pare-feux FortiGate via les profils AntiVirus (voir [README](https://github.com/romainmarcoux/malicious-hash))

Caractéristiques communes de toutes les agrégations :

- Mise à jour toutes les **heures**
- **Lire attentivement** le README de chaque dépôt Github qui contient :
  * Le nombre d'éléments
  * La **méthode d'implémentation**
  * Les liens des différents fichiers
  * Les sources agrégées
  * Les évolutions effectuées
- Les éléments sont ordonnés en fonction du nombre de sources dans lesquelles ils apparaissent :
  * Un élément apparaissant dans le plus de sources est donc dans le début du premier fichier

Si vous utilisez mes agrégations, n'hésitez pas à vous connecter à mon [profil](https://linkedin.com/in/romainmarcoux/) LinkedIn et m'envoyer un message pour :
- me remercier et m'encourager 😉
- que je vous prévienne des évolutions et des nouveaux segments à ajouter dans vos systèmes
- me prévenir d'erreurs, problèmes, faux positifs ou d'IP / entrées DNS malveillantes qui seraient absentes de mes agrégations
- me solliciter pour bénéficier de mon expertise en cybersécurité (audit, conseil, intégration) que je propose en tant que __freelance__ à des **clients finaux** et en sous-traitance à des **partenaires** en manque de ressources ou d'expertise. Plus d'infos sur mon [profil](https://linkedin.com/in/romainmarcoux/) LinkedIn. 

# [EN] Infos

This GitHub provides aggregations of **IP addresses, domains and malicious hashes** ready to be implemented on your security systems: firewalls (notably FortiGate), web servers, WAF, proxy, etc.
- [malicious-ip](https://github.com/romainmarcoux/malicious-ip) : aggregation of malicious IP addresses (scanners, bruteforce, etc.) to be blocked at **input** (WAN > LAN)
- [malicious-domains](https://github.com/romainmarcoux/malicious-domains) : aggregation of malicious domains (phishing / phishing, malware, etc.) to be blocked on **output** (LAN > WAN)
- [malicious-hash](https://github.com/romainmarcoux/malicious-hash) : aggregation of hashes of malicious files (on FortiGate firewalls, can be implemented in AntiVirus profiles)

Common characteristics of all aggregations:

- Updated every **hour**
- **Read carefully** the README of each Github repository which contains:
   * The number of elements
   * The **implementation method**
   * Links to different files
   * Aggregated sources
   * The developments carried out
- Elements are ordered according to the number of sources in which they appear:
   * An element appearing in the most sources is therefore at the beginning of the first file

If you use my aggregations, feel free to connect to my LinkedIn [profile](https://linkedin.com/in/romainmarcoux/) and send me a message to:
- thank me and encourage me 😉
- that I notify you of developments and new segments to be added to your systems
- warn me of errors, problems, false positives or malicious IP / DNS entries that are missing from my aggregations
- ask me to benefit from my expertise in cybersecurity (audit, consulting, integration) which I offer as a __freelance__ to **end clients** and as a subcontractor to **partners** lacking resources or expertise. More info on my LinkedIn [profile](https://linkedin.com/in/romainmarcoux/).
