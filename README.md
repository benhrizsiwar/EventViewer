# EventViewer
# Fichiers de configuration de surveillance DNS

Ce dépôt contient un fichier de configuration XML pour la surveillance des événements DNS sur un système Windows. Ce fichier XML est conçu pour collecter des événements provenant de différentes sources, telles que le **Microsoft-Windows-DNS-Client** et **Microsoft-Windows-Narrator**, ainsi que des événements liés aux ID spécifiés dans la section `<EventId>`.

## Vue personnalisée

Le fichier `dns-query-config.xml` contient une configuration détaillée permettant de filtrer les événements suivant ces critères :
- **Sources** : Microsoft-Windows-DNS-Client et Microsoft-Windows-Narrator
- **Niveau des événements** : Les événements sont filtrés pour les niveaux de 1 à 4 et 0.
- **ID des événements** : Les événements spécifiés incluent des ID allant de 2, 4, 409, et d'autres ID allant de 501 à 502 et de 6001 à 6002.

Cette configuration est utilisée pour collecter les événements spécifiques à la surveillance du client DNS, utile pour les administrateurs réseau et les diagnostics.

## Utilisation

Pour utiliser cette configuration, vous devez l'intégrer dans votre système de surveillance Windows, où elle interrogera les journaux d'événements associés et en extraiera les informations pertinentes basées sur la configuration définie.

## Installation

1. Téléchargez le fichier `Surveillance DNS.xml` depuis ce dépôt.
2. Ajoutez-le à votre configuration de surveillance d'événements.

## Contributions

Les contributions sont les bienvenues. Si vous avez des suggestions ou des améliorations, n'hésitez pas à créer une **Pull Request**.

