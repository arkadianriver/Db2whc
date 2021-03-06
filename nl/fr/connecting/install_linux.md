---

copyright:
  years: 2014, 2018
lastupdated: "2018-09-25"

---

<!-- Attribute definitions --> 
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:pre: .pre}

# Installation du module de pilote sur Linux ou PowerLinux

Vous pouvez installer le module de pilote {{site.data.keyword.dashdbshort_notm}} sur Linux ou PowerLinux avec `installDSDriver`.
{: shortdesc}

## Prérequis

Avant de tenter une connexion à votre base de données {{site.data.keyword.dashdbshort_notm}}, vérifiez que les [conditions requises](connecting.html#prereqs) sont remplies.

<!-- Download the Db2 driver package for your operating system from the web console and install it. -->

**Sur PowerLinux uniquement**, effectuez les étapes suivantes pour installer le module d'exécution du compilateur XL C/C++ :

1. Téléchargez le module d'exécution du compilateur XL C/C++ du site FTP. Par exemple, pour utiliser l'outil **wget** pour télécharger le module d'exécution pour Linux little endian Ubuntu 14, exécutez la commande suivante : 

   `wget ftp://public.dhe.ibm.com/software/server/POWER/Linux/rte/xlcpp/le/ubuntu/dists/trusty/main/binary-ppc64el/*`
2. Installez le module d'exécution en exécutant la commande suivante :

   `sudo dpkg -iG *.deb` 

## Procédure

1. Décompressez le fichier de module de pilote compressé que vous venez de télécharger.

   Exemple : 

   `gunzip file_name.tar.gz`

   `tar -xvf file_name.tar`

    Un sous-répertoire `dsdriver` est créé dans le répertoire où vous avez exécuté les commandes de décompression.
2. Extrayez les pilotes Java et ODBC/CLI.

   a. Dans le sous-répertoire `dsdriver`, exécutez la commande **installDSDriver**.
   
   La commande **installDSDriver** crée les fichiers script `db2profile` et `db2cshrc` dans le répertoire `dsdriver`.

   b. Exécutez l'un des fichiers script suivants en fonction de votre environnement shell :

   - **shell Bash ou Korn shell** : `source db2profile`
   - **shell C** : `source db2cshrc`

## Que faire ensuite ?

Pour pouvoir connecter vos applications locales ou vos outils clients à votre base de données {{site.data.keyword.dashdbshort_notm}}, [configurez votre environnement local](driver_pkg_cfg.html).   




