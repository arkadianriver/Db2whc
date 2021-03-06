---

copyright:
  years: 2014, 2019
lastupdated: "2018-04-30"

---

<!-- Attribute definitions --> 
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:important: .important}
{:note: .note}
{:deprecated: .deprecated}
{:pre: .pre}

# High availability (HA) 
{: #ha}

The measure of a successful database solution is its availability. {{site.data.keyword.dashdblong}} has highly available plans to keep your workloads going.
{: shortdesc}

## MPP plan
{: #ha_mpp}

The {{site.data.keyword.dashdbshort_notm}} MPP plan cluster is provisioned with high availability.  

When a node goes down for an MPP plan, the HA component restarts your database partitions in the remaining healthy nodes. A short downtime occurs during this phase. 

After the node is added back to the cluster, the database engine must be restarted to run at full capacity. 

## Flex Performance plan
{: #ha_flex}

If an unexpected node failure does occur, your Flex Performance MPP cluster is brought back to full capacity after a short downtime due to using the IBM Container Service (based on Kubernetes). Nodes from a pool are used to move the failed node entities. 

### Compute HA
{: #compute_ha}

Any node failure is immediately detected by the container service. The containers and pods that were running in the failed node are scheduled to a new node from a pool of nodes. The system is back to 100% normal operation after a short downtime.

### Storage HA
{: #storage_ha}

Your storage is configured with a dual-parity RAID6 implementation that provides protection against double disk failures in the same RAID group for high performance and highly available storage for your system.

### Network HA
{: #net_ha}

Network connections are made highly available by provisioning your service with a redundant network interface card (NIC). 

If the container service detects a network issue, pods and containers can automatically restart after a short downtime.