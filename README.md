# TP-Cybers-curit-Configuration-d-un-pare-feu-UFW

## Objectif

Configurer un pare-feu UFW sur un serveur Linux afin de limiter les accès réseau.

## Contexte

Un serveur ne doit exposer que les services nécessaires.  
Le pare-feu permet de bloquer les connexions non autorisées.

## Règles mises en place

- Autoriser SSH
- Autoriser HTTP
- Autoriser HTTPS
- Bloquer le reste du trafic entrant

## Commandes principales

```bash
ufw default deny incoming
ufw default allow outgoing
ufw allow OpenSSH
ufw allow 80/tcp
ufw allow 443/tcp
ufw enable
ufw status verbose
