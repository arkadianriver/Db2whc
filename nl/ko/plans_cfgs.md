---

copyright:
  years: 2014, 2018
lastupdated: "2018-10-24"

---

<!-- Attribute definitions --> 
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:pre: .pre}

# 플랜 및 구성
{: #plans_cfgs}

수행해야 하는 작업에 맞게 구성되고 최적화된 {{site.data.keyword.dashdbshort_notm}} 플랜을 선택할 수 있습니다.
{: shortdesc}

   * 테스트를 위한 엔트리 플랜. 최대 1GB의 저장 공간을 갖춘 무료 평가판입니다.
   * 스토리지 및 컴퓨팅 리소스를 독립적으로 스케일링할 수 있는 Flex 플랜
   * 다양한 크기의 프로덕션을 위한 SMP 플랜: 단일 노드 및 단일 인스턴스로 구성된 소형, 중형 및 대형
   * 병렬 처리 및 고성능용 MPP 다중-노드 클러스터 구성
   * 고가용성을 위해 구성된 플랜
   * Oracle 호환성

[{{site.data.keyword.Bluemix}} 카탈로그](https://console.bluemix.net/catalog/services/db2-warehouse){:new_window}에서 모든 사용 가능한 {{site.data.keyword.dashdbshort_notm}} 플랜을 보십시오.
<!--   * Plans configured for data warehouse and online analytical processing (OLAP) workloads: [{{site.data.keyword.dashdbshort_notm}}](https://console.bluemix.net/catalog/services/db2-warehouse){:new_window} -->
<!--   * Plans configured for high-speed, transactional processing (OLTP): [{{site.data.keyword.dashdbshort_notm}} for Transactions](https://console.ng.bluemix.net/catalog/services/dashdb-for-transactions-sql-database){:new_window} -->

{{site.data.keyword.dashdbshort_notm}} Flex Performance 플랜에 대한 소개를 보려면 이 동영상을 시청하십시오.

<iframe class="embed-responsive-item" id="youtubeplayer" title="Cognos Analytics에서 연결 작성" type="text/html" width="640" height="390" src="//www.youtube.com/embed/59PKSnzNQAg?rel=0" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen> </iframe>

{{site.data.keyword.dashdbshort_notm}} 서비스를 {{site.data.keyword.Bluemix}}의 네트워크 격리 환경에 배치하도록 요청할 수 있습니다. [{{site.data.keyword.IBM_notm}} 영업 팀 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://www.ibm.com/connect/ibm/us/en/?lnk=fcw){:new_window}에 문의하십시오.

카탈로그에서 필요한 구성을 찾을 수 없는 경우 [{{site.data.keyword.IBM_notm}} 영업 팀 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://www.ibm.com/connect/ibm/us/en/?lnk=fcw){:new_window}에 문의하여 다른 옵션에 대해 논의하십시오.

## 데이터 센터의 플랜 가용성
{: #availability}

다음 표는 실제 지역에 있는 데이터 센터에서 제공하는 다양한 Db2 Warehouse on Cloud 플랜의 가용성에 대한 정보를 제공합니다.

| Db2 Warehouse on Cloud 플랜 | 아시아/태평양 | 유럽    | 북/중앙아메리카     | 남아메리카 |
|------------------------------|--------------|-----------|-----------------------    |---------------|
| Flex                         | *NA          | 프랑크푸르트 | 워싱턴 D.C.(미국 동부) | *NA           |
|                              |              |           | 댈러스(미국 남부)         |               |  
|      |||||
| SMP                          | 홍콩    | 암스테르담 | 워싱턴 D.C.(미국 동부) | 상파울루     |
|                              | 서울        | 프랑크푸르트 | 댈러스(미국 남부)         |               | 
|                              | 싱가포르    | 런던    | 몬트리올                  |               | 
|                              | 시드니       | 밀라노     | 케레타로                 |               | 
|                              | 도쿄        | 오슬로      | 토론토                   |               | 
|                              |              | 파리     |                           |               |
|      |||||
| MPP                          | 홍콩    | 암스테르담 | 워싱턴 D.C.(미국 동부) | 상파울루     |
|                              | 서울        | 프랑크푸르트 | 댈러스(미국 남부)         |               | 
|                              | 싱가포르    | 런던    | 몬트리올                  |               | 
|                              | 시드니       | 밀라노     | 케레타로                 |               | 
|                              | 도쿄        | 오슬로      | 토론토                   |               | 
|                              |              | 파리     |                           |               |
{: caption="표 1. Db2 Warehouse on Cloud 서비스 플랜을 지원하는 데이터 센터" caption-side="top"}

*NA = 현재 사용할 수 없음



