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

# Conexión mediante programa con JDBC

Defina una conexión entre una aplicación Java™ y la base de datos de {{site.data.keyword.dashdbshort_notm}}.
{: shortdesc}

## Requisitos previos

Antes de intentar realizar una conexión a su base de datos de {{site.data.keyword.dashdbshort_notm}}, verifique que dispone de los [requisitos previos](connecting.html#prereqs) necesarios.

<!-- Before you can connect to your database, you must perform the following steps:

- [Verify prerequisites](prereqs.html), including installing driver packages, configuring your local environment, and downloading SSL certificates (if needed)
- Collect [connection information](credentials.html), including database details such as host name and port numbers, and connection credentials such as user ID and password -->

## Procedimiento

En cada aplicación Java, especifique el ID de usuario y la contraseña incluyendo el método **DriverManager.getConnection** y, a continuación, incluya una de las series URL JDBC siguientes:

- Para una conexión con SSL:

  `jdbc:db2://<host_name>:50001/BLUDB:sslConnection=true;`

- Para una conexión sin SSL:

  `jdbc:db2://<host_name>:50000/BLUDB`


