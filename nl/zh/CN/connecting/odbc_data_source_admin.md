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

# 使用 ODBC 数据源管理器进行连接

使用 Microsoft ODBC 数据源管理器工具来定义 ODBC 应用程序或 CLI 应用程序与 {{site.data.keyword.dashdbshort_notm}} 数据库之间的连接。
{: shortdesc}

## 先决条件

在尝试连接到 {{site.data.keyword.dashdbshort_notm}} 数据库之前，请验证您是否具有必需的[先决条件](connecting.html#prereqs)。

<!-- Before you can connect to your database, you must perform the following steps:

- [Verify prerequisites](prereqs.html), including installing driver packages, configuring your local environment, and downloading SSL certificates (if needed)
- Collect [connection information](credentials.html), including database details such as host name and port numbers, and connection credentials such as user ID and password -->

## 过程

1. 安装 [Db2 驱动程序包](driver_pkg.html)。

2. 打开 ODBC 数据源管理器，并为 Db2 驱动程序包创建“用户 DSN”或“系统 DSN”。
    
3. 单击**高级设置**。针对 {{site.data.keyword.dashdbshort_notm}} 服务器，输入以下 CLI 参数的值：**主机名**、**端口**和**数据库**。
    
4. 对于 SSL 连接，请为 CLI 参数**安全性**输入值 `SSL`。
    
5. 单击**应用**。
    
6. 要测试连接，请返回到 ODBC 数据源管理器的主页。针对所创建的 DSN，单击**配置**。输入服务器的用户标识和密码，然后单击**连接**。

