# Investigation d'une adresse IP

## Description

Ce projet présente l'investigation d'une adresse IP publique.

L'objectif était d'identifier les services accessibles et d'analyser le comportement du service HTTPS.

## Outils utilisés

- Nmap
- OpenSSL
- Curl
- Netcat
- Whois

## Ce qui a été étudié

- Les ports accessibles.
- Les services exposés.
- HTTPS et TLS.
- Le SNI.
- Les Virtual Hosts.
- Les certificats TLS.

## Résultat

L'analyse a permis d'identifier un service HTTPS dont le comportement dépendait du nom envoyé via le SNI.

Un mauvais nom provoquait une erreur TLS, tandis qu'un nom reconnu permettait au serveur de présenter son certificat.

## Avertissement

Ce projet est réalisé dans un cadre éducatif. Les techniques présentées doivent être utilisées uniquement sur des systèmes autorisés.
