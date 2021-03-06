﻿---
title: 'UM 사서함 정책: Exchange 2013 Help'
TOCTitle: UM 사서함 정책
ms:assetid: dfae629e-ee89-4494-a3ed-9655b67eb87e
ms:mtpsurl: https://technet.microsoft.com/ko-kr/library/Bb124909(v=EXCHG.150)
ms:contentKeyID: 50556097
ms.date: 05/22/2018
mtps_version: v=EXCHG.150
ms.translationtype: MT
---

# UM 사서함 정책

 

_**적용 대상:** Exchange Online, Exchange Server 2013, Exchange Server 2016_

_**마지막으로 수정된 항목:** 2012-11-15_

통합 메시징 (UM) 사서함 정책을 사용자가 통합 메시징을 사용 하도록 설정 하는 경우에 필요 합니다. 음성 메일 사용자의 사서함의 컬렉션에 정책 또는 보안 설정의 공통 집합을 적용 하려면 UM 사서함 정책을 만듭니다. UM 사서함 정책 다음과 같은 UM 설정을 지정 하는데 사용 됩니다.

  - PIN 정책

  - 전화 걸기 제한

  - 기타 일반적인 UM 사서함 정책 속성

예 임원 등의 UM 사용이 가능한 사용자의 특정 그룹에 대 한 로그인 실패의 최대 수를 줄여 PIN 보안 수준을 높일 수 UM 사서함 정책을 만들 수 있습니다.

## UM 사서함 정책

통합 메시징에 대 한 사용자를 설정 하기 전에 하나 이상의 UM 사서함 정책을 만든 것 이어야 합니다. 공통 사용자 그룹에 대 한 설정 집합을 적용 하려면 추가 UM 사서함 정책을 만들 수 있습니다.

Exchange 관리 셸 또는 Exchange 관리 센터 (EAC)를 사용 하 여 UM 사서함 정책을 만듭니다. 기본적으로 단일 UM 사서함 정책에는 UM 다이얼 플랜을 만들 때마다 만들어집니다. 새 UM 사서함 정책 UM 다이얼 플랜과 자동으로 연결 이며 다이얼 플랜 이름의 일부 UM 사서함 정책의 표시 이름에 포함 됩니다. 이 기본 UM 사서함 정책을 편집할 수 있습니다.

여러 UM 사용이 가능한 사용자가 단일 UM 사서함 정책에 연결할 수 있습니다. 그러나 각 UM 사용이 가능한 사용자에 대 한 사서함은 단일 UM 사서함 정책에 연결 되어야 합니다. 이렇게 하면 PIN 보안 설정 예: PIN의 최소 자릿수 또는 UM 사용이 가능한 사용자에 연결 된 UM 사서함 정책에 대 한 로그인 시도의 최대 수를 제어 합니다. 메시지 텍스트 설정 또는 동일한 UM 사용이 가능한 사서함에 대 한 전화를 걸 제한을 제어할 수 있습니다.

