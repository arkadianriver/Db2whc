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

# Connexion à ODBC Data Source Administrator

Utilisez l'outil ODBC Data Source Administrator de Microsoft pour définir une connexion entre une application d'interface de ligne de commande ou une application ODBC et une base de données {{site.data.keyword.dashdbshort_notm}}.
{: shortdesc}

## Prérequis

Avant de tenter une connexion à votre base de données {{site.data.keyword.dashdbshort_notm}}, vérifiez que les [conditions requises](connecting.html#prereqs) sont remplies.

<!-- Before you can connect to your database, you must perform the following steps:

- [Verify prerequisites](prereqs.html), including installing driver packages, configuring your local environment, and downloading SSL certificates (if needed)
- Collect [connection information](credentials.html), including database details such as host name and port numbers, and connection credentials such as user ID and password -->

## Procédure

1. Installez le [module de pilote Db2](driver_pkg.html).

2. Ouvrez ODBC Data Source Administrator et créez un DSN utilisateur ou un DSN système pour le module de pilote Db2.
    
3. Cliquez sur **Paramètres avancés**. Entrez les paramètres d'interface de ligne de commande suivants avec leurs valeurs pour le serveur {{site.data.keyword.dashdbshort_notm}} : **Nom d'hôte**, **Port** et **Base de données**.
    
4. Pour une connexion SSL, entrez le paramètre d'interface de ligne de commande **Sécurité** avec la valeur `SSL`.
    
5. Cliquez sur **Appliquer**.
    
6. Pour tester la connexion, retournez à la page principale d'ODBC Data Source Administrator. Cliquez sur **Configurer** pour le DSN que vous avez créé. Entrez l'ID d'utilisateur et le mot de passe du serveur et cliquez sur **Connecter**.

