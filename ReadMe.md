## Introduction
Dans le cadre du projet "Intégration des Services et des Objets", notre initiative se concentre sur la modélisation et la mise en place des processus de gestion des missions attribuées aux professeurs et aux administrateurs, en adoptant une approche basée sur l'architecture Orientée Service (SOA). Notre but est de concevoir un système qui permettra de gérer de manière optimale toutes les étapes liées à la gestion des divers processus liés aux missions.

Dans cette perspective, nous débuterons par une modélisation des processus en utilisant le langage de modélisation BPMN (Business Process Model and Notation). Cette étape permettra une visualisation claire des interactions et des séquences d'activités au sein des processus de gestion des missions.

Nous avons choisi la plateforme MuleSoft pour le développement du backend, qui facilitera la communication entre les services et assurera une orchestration efficace des processus métier. L'utilisation de cette technologie SOA moderne garantira la souplesse et la scalabilité nécessaires à l'évolution du système. Le développement de l'interface utilisateur se fera avec le framework React, offrant une expérience utilisateur moderne et réactive, facilitant l'interaction avec le système de gestion des missions. La gestion des données sera assurée par une base de données MySQL, responsable du stockage efficace et sécurisé des informations relatives aux missions, contribuant à la robustesse globale du système.

Ainsi,  notre projet s'appuie sur une approche intégrée, allant de la modélisation précise des processus en BPMN, à l'utilisation de MuleSoft pour l'orchestration des services backend, et enfin à la conception d'une interface utilisateur interactive avec React, le tout soutenu par une base de données MySQL pour garantir la persistance des données. Cette approche intégrée vise à créer une solution complète et performante pour la gestion des missions au sein de l'ENSIAS.


## Contexte du Projet :
Application Workflow de gestion des missions des professeurs/Administrateurs de l'ENSIAS représente une solution basée sur l'architecture SOA, intégrant la technologie BPEL pour orchestrer les processus métier. Cette application vise à simplifier les tâches complexes et répétitives, offrant aux utilisateurs la flexibilité nécessaire pour adapter les processus selon leurs besoins spécifiques.
Au cœur de cette application se trouve le moteur BPEL, qui assure l'exécution efficace des processus métier définis dans un modèle ajustable. Ces processus peuvent englober diverses activités, telles que la création et la modification de documents, la gestion des flux de travail, le traitement des demandes, et l'exécution d'autres processus métier.
Les avantages offerts par ce système sont nombreux, parmi lesquels on peut citer :

- Gestion Complète des Demandes de mission et de remboursement.
- Toutes les demandes sont centralisées, facilitant la gestion et l'accès aux informations.
- L'application génère automatiquement des états détaillés des sommes dues aux frais de déplacement.
- Chaque étape du processus de gestion des missions est tracée, offrant une visibilité complète.


## Macro-processus de la gestion des missions et de remboursements : 

<p align="center" >
<img src= "Resource/macro_process.png" height="180" width="auto" />
</p>

## Acteurs du système :

- Professeur/Administrateur

- Chef Immédiatier approbateur d'une demande avant de la transmettre aux autres acteurs.

- Régisseur
 
## Modélisation des processus : 

<p align="center" >
<img src= "Resource/mission.png" height="180" width="auto" />
</p>
Modélisation du processus de création d’une demande de mission
<p align="center" >
<img src= "Resource/remboursement.png" height="180" width="auto" />
</p>
Modélisation du processus de demande d’un remboursement

## Architecture Orientée Services (SOA) :
En optant pour une Architecture Orientée Services (SOA), nous procédons à la décomposition du système global en services modulaires et autonomes. Chaque service représente une fonction spécifique, telle que la soumission de demande de mission, les workflows d'approbation, le traitement des remboursements et la génération de rapports. Cette approche modulaire permet à chaque service d'évoluer indépendamment, conférant au système une adaptabilité accrue aux exigences changeantes.

## Solution d'Intégration :
Après la conception de l'application et de sa logique, notre objectif est maintenant de concevoir et de mettre en œuvre une solution d'intégration au sein du bus de services d'entreprise (ESB) fourni par MuleSoft. Cette solution va connecter différents services impliqués dans les processus décrits précédemment. L'intégration englobera le partage de données, la communication basée sur des événements et l'établissement de protocoles standardisés afin de garantir un système cohérent et interopérable.