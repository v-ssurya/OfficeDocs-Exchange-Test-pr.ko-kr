﻿---
title: '메일 사용자 관리: Exchange 2013 Help'
TOCTitle: 메일 사용자 관리
ms:assetid: bb8b8804-f730-4ad7-9173-896a4965b90f
ms:mtpsurl: https://technet.microsoft.com/ko-kr/library/Bb124381(v=EXCHG.150)
ms:contentKeyID: 50482288
ms.date: 05/22/2018
mtps_version: v=EXCHG.150
f1_keywords:
- Microsoft.Exchange.Management.SnapIn.Esm.Recipients.NewMailUserWizardForm.NewMailUserIntroductionWizardPage
ms.translationtype: MT
---

# 메일 사용자 관리

 

_**적용 대상:**Exchange Online, Exchange Server 2013_

_**마지막으로 수정된 항목:**2016-12-09_

메일 사용자는 메일 연락처와 비슷합니다. 둘 다 외부 전자 메일 주소가 있고 Exchange 또는 Exchange Online 조직 외부에 있는 사람에 대한 정보를 포함하며 공유 주소록과 기타 주소 목록에 표시될 수 있습니다. 그러나 메일 사용자는 메일 연락처와 달리 Exchange 또는 Office 365 조직 로그온 자격 증명이 있으며 리소스에 액세스할 수 있습니다. 자세한 내용은 [받는 사람](recipients-exchange-2013-help.md)을 참조하십시오.

## 시작하기 전에 알아야 할 내용

  - 예상 완료 시간: 2분.

  - 이러한 절차를 수행하려면 먼저 사용 권한을 할당받아야 합니다. 필요한 사용 권한을 확인하려면 다음을 참조하세요. [받는 사람에 게 사용 권한](recipients-permissions-exchange-2013-help.md)의 "받는 사람의 프로비전 권한" 섹션

  - 이 항목의 절차에 적용할 수 있는 바로 가기 키에 대한 자세한 내용은 [Exchange 관리 센터의 바로 가기 키](keyboard-shortcuts-in-the-exchange-admin-center-exchange-online-protection-help.md)을 참조하세요.


> [!TIP]
> 문제가 있습니까? Exchange 포럼에서 도움을 요청하세요. 포럼 주소는 다음과 같습니다. <A href="https://go.microsoft.com/fwlink/p/?linkid=60612">Exchange Server</A>, <A href="https://go.microsoft.com/fwlink/p/?linkid=267542">Exchange Online</A>, 또는 <A href="https://go.microsoft.com/fwlink/p/?linkid=285351">Exchange Online Protection</A>.



## 무슨 작업을 하고 싶으십니까?

## 메일 사용자 만들기

## EAC를 사용하여 메일 사용자 만들기

1.  EAC에서 **받는 사람** \> **연락처** \> **새로 만들기** \> **메일 사용자**로 이동합니다.

2.  **새 메일 사용자** 페이지의 **\* 별칭** 입력란에 메일 사용자의 별칭을 입력합니다. 별칭은 64자를 초과할 수 없으며 포리스트에서 고유해야 합니다. 이 입력란은 필수입니다.

3.  메일 사용자의 전자 메일 주소를 지정하려면 다음 중 하나를 수행하십시오.
    
      - 메일 사용자의 외부 전자 메일 주소에 대한 SMTP 전자 메일 주소를 지정하려면 **SMTP**를 클릭합니다.
        

        > [!NOTE]
        > Exchange에서 SMTP 주소의 형식이 올바른지 유효성을 검사합니다. 입력 내용이 SMTP 형식과 일치하지 않을 경우 메일 사용자를 만들기 위해 <STRONG>저장</STRONG>을 클릭하면 오류 메시지가 표시됩니다.

    
      - 사용자 지정 주소 형식을 지정하려면 옵션 단추를 클릭하고 사용자 지정 주소 형식을 입력합니다. 예를 들면, X.500, GroupWise 또는 Lotus Notes 주소를 지정할 수 있습니다.

4.  **\* 외부 전자 메일 주소** 입력란에 메일 사용자의 외부 전자 메일 주소를 입력합니다. 이 메일 사용자에게 보낸 전자 메일이 이 전자 메일 주소로 전달됩니다. 이 입력란은 필수입니다.

5.  
    
    다음 옵션 중 하나를 선택합니다.
    
      - **기존 사용자**   기존 사용자가 메일을 사용하도록 설정하려면 선택합니다.
        
        **찾아보기**를 클릭하여 **사용자 선택 – 전체 포리스트** 대화 상자를 엽니다. 이 대화 상자에는 조직에서 메일을 사용하도록 설정되지 않았거나 사서함이 없는 사용자 계정 목록이 표시됩니다. 메일을 사용할 수 있도록 설정할 사용자 계정을 선택하고 **확인**을 클릭합니다. 이 옵션을 선택할 경우 사용자 계정 정보를 제공할 필요가 없습니다. 이 정보는 Active Directory에도 이미 있기 때문입니다.
    
      - **새 사용자**   Active Directory에 새 사용자 계정을 만들고 사용자가 메일을 사용하도록 하려면 선택합니다. 이 옵션을 선택하면 필요한 사용자 계정 정보를 제공해야 합니다.

6.  
    
    5단계에서 **새 사용자**를 선택한 경우 **새 메일 사용자** 페이지의 다음 입력란에 해당 정보를 입력합니다. 그렇지 않으면 7단계로 건너뜁니다.
    
      - **이름**   이 입력란에 메일 사용자의 이름을 입력합니다.
    
      - **이니셜**   이 입력란에 메일 사용자의 이니셜을 입력합니다.
    
      - **성**   이 입력란에 메일 사용자의 성을 입력합니다.
    
      - **\* 표시 이름**   이 입력란에 사용자의 표시 이름을 입력합니다. EAC의 연락처 목록 및 조직의 주소록에 표시되는 이름입니다. 기본적으로 이 상자에는 **이름**, **이니셜** 및 **성** 상자에 입력한 이름이 채워집니다. 해당 입력란을 사용하지 않은 경우에도 이 입력란은 필수이므로 이름을 입력해야 합니다. 이름은 64자를 초과할 수 없습니다.
    
      - **\* 이름**   이 입력란에 메일 사용자의 이름을 입력합니다. 이 이름은 디렉터리 서비스에 나열된 이름입니다. 이 입력란에도 **이름**, **이니셜** 및 **성** 상자에 입력한 이름이 채워집니다. 해당 입력란을 사용하지 않은 경우에도 이 입력란은 필수이므로 이름을 입력해야 합니다. 이 이름 역시 64자를 초과할 수 없습니다.
        

        > [!NOTE]
        > <STRONG>이름</STRONG> 상자는 Exchange Server 2013에서만 사용할 수 있으며 Exchange Online에서는 사용할 수 없습니다.

    
      - **조직 구성 단위**   기본값(받는 사람 범위) 이외의 OU(조직 구성 단위)를 선택할 수 있습니다. 받는 사람 범위가 포리스트로 설정되어 있으면 기본값은 EAC를 실행 중인 컴퓨터가 포함된 도메인의 사용자 컨테이너로 설정됩니다. 받는 사람 범위가 특정 도메인으로 설정되어 있으면 해당 도메인의 사용자 컨테이너가 기본적으로 선택됩니다. 받는 사람 범위가 특정 OU로 설정되어 있으면 해당 OU가 기본적으로 선택됩니다.
        
        다른 OU를 선택하려면 **찾아보기**를 클릭합니다. 이 대화 상자에는 지정된 범위 내에 있는 포리스트의 모든 OU가 표시됩니다. 원하는 OU를 선택한 다음 **확인**을 클릭합니다.
        

        > [!NOTE]
        > <STRONG>조직 구성 단위</STRONG> 상자는 Exchange Server 2013에서만 사용할 수 있습니다. Exchange Online에서는 사용할 수 없습니다.

    
      - **\* 사용자 로그온 이름**   메일 사용자가 도메인에 로그온할 때 사용할 이름을 입력합니다. 사용자 로그온 이름은 @ 기호 왼쪽의 사용자 이름과 오른쪽의 접미사로 구성됩니다. 일반적으로 접미사는 사용자 계정이 있는 도메인 이름입니다.
        

        > [!NOTE]
        > Exchange Online에서는 이 입력란의 레이블이 <STRONG>사용자 ID</STRONG>입니다.

    
      - **\* 새 암호**   이 입력란에 메일 사용자가 도메인에 로그온할 때 사용해야 할 암호를 입력합니다.
        

        > [!NOTE]
        > 입력하는 암호는 사용자 계정을 만들 도메인의 암호 길이, 복잡성 및 내역 요구 사항을 준수해야 합니다.

    
      - **\* 암호 확인**   **암호** 상자에 입력한 암호를 이 입력란에 다시 입력하여 확인합니다.
    
      - **다음 로그온 시 암호 변경 필요**   메일 사용자가 도메인에 처음으로 로그온할 때 암호를 다시 설정하도록 하려면 이 확인란을 선택합니다.
        
        이 확인란을 선택하면 새 메일 사용자가 처음 로그온할 때 암호를 변경하라는 대화 상자가 표시됩니다. 메일 사용자는 암호를 변경해야 작업을 수행할 수 있습니다.

7.  
    
    모든 설정이 끝나면 **저장**을 클릭하여 메일 사용자를 만듭니다.

## 셸을 사용하여 메일 사용자 만들기

이 예에서는 다음 세부 정보를 사용하여 Exchange Server 2013에서 Jeffrey Zeng에 대한 메일 사용이 가능한 사용자 계정을 만듭니다.

  - 이름과 표시 이름은 Jeffrey Zeng입니다.

  - 별칭은 jeffreyz입니다.

  - 외부 전자 메일 주소는 jzeng@tailspintoys.com입니다.

  - 이름은 Jeffrey고 성은 Zeng입니다.

  - 로그온 이름은 jeffreyz@contoso.com입니다.

  - 암호는 Pa$$word1입니다.

  - 메일 사용자는 기본 OU에서 만들어집니다. 다른 OU를 지정하려면 *OrganizationalUnit* 매개 변수를 사용하면 됩니다.

<!-- end list -->

    New-MailUser -Name "Jeffrey Zeng" -Alias jeffreyz -ExternalEmailAddress jzeng@tailspintoys.com -FirstName Jeffrey -LastName Zeng -UserPrincipalName jeffreyz@contoso.com -Password (ConvertTo-SecureString -String 'Pa$$word1' -AsPlainText -Force)

이 예에서는 Exchange Online에서 Rene Valdes에 대한 메일 사용이 가능한 사용자 계정을 만듭니다.

    New-MailUser -Name "Rene Valdes" -Alias renev -ExternalEmailAddress renevaldes@fineartschool.edu -FirstName Rene -LastName Valdes -MicrosoftOnlineServicesID renev@contoso.com -Password (ConvertTo-SecureString -String 'P@ssw0rd' -AsPlainText -Force)

## 작동 여부는 어떻게 확인합니까?

메일 사용자가 만들어졌는지 확인하려면 다음 중 하나를 수행합니다.

  - EAC에서 **받는 사람** \> **연락처**로 이동합니다. 새 메일 사용자가 연락처 목록에 표시됩니다. **연락처 유형**에 유형이 **메일 사용자**로 표시됩니다.

  - 셸에서 다음 명령을 실행하여 새 메일 사용자에 대한 정보를 표시합니다.
    
        Get-MailUser <Name> | FL Name,RecipientTypeDetails,ExternalEmailAddress

## 메일 사용자 속성 변경

메일 사용자를 만든 후 EAC 또는 셸을 사용하여 설정을 변경하거나 추가 속성을 설정할 수 있습니다.

여러 사용자 사서함의 속성을 동시에 변경할 수도 있습니다. 자세한 내용은 Bulk edit mail users을 참조하십시오.

이 작업의 예상 완료 시간은 보거나 변경하려는 속성 수에 따라 다릅니다.

## EAC를 사용하여 사용자 사서함 속성 변경

1.  EAC에서 **받는 사람** \> **연락처**로 이동합니다.

2.  연락처 목록에서 속성을 변경할 메일 사용자를 클릭한 다음 **편집**![편집 아이콘](images/JJ218640.6f53ccb2-1f13-4c02-bea0-30690e6ea71d(EXCHG.150).gif "편집 아이콘")을 클릭합니다.

3.  메일 사용자 속성 페이지에서 다음 섹션 중 하나를 클릭하여 속성을 보거나 변경합니다.
    
      - General
    
      - Contact Information
    
      - Organization
    
      - Email Addresses
    
      - Mail Flow Settings
    
      - Member Of
    
      - MailTip

## 일반

메일 사용자에 대한 기본 정보를 보거나 변경하려면 **일반** 섹션을 사용합니다.

  - **이름**, **이니셜**, **성**

  - **\* 이름**   Active Directory에 표시되는 이름입니다. 이 이름을 변경하는 경우 64자를 초과할 수 없습니다.

  - **\* 표시 이름**    이 이름은 조직의 주소록, 전자 메일의 받는 사람: 및 보낸 사람: 줄 및 EAC의 연락처 목록에 표시됩니다. 표시 이름 앞뒤에는 빈 공간을 포함할 수 없습니다.

  - **\* 사용자 로그온 이름**   사용자가 도메인에 로그온할 때 사용하는 이름입니다. Exchange Online에서 이 이름은 사용자가 Office 365에 로그인하는 데 사용하는 사용자 ID입니다.

  - **주소 목록에서 숨기기**    Exchange 조직에 정의된 주소록 및 다른 주소 목록에 메일 사용자가 표시되지 않도록 하려면 이 확인란을 선택합니다. 이 확인란을 선택한 후에도 사용자는 전자 메일 주소를 사용하여 받는 사람에게 메시지를 보낼 수 있습니다.

  - **다음 로그온 시 암호 변경 필요**   사용자가 다음에 도메인에 로그온할 때 암호를 다시 설정하도록 하려면 이 확인란을 선택합니다.
    

    > [!NOTE]
    > Exchange Online에서는 이 확인란을 사용할 수 없습니다.



다음과 같은 추가 속성을 보거나 변경하려면 **기타 옵션**을 클릭합니다.

  - **조직 구성 단위**   이 읽기 전용 상자에는 메일 사용자 계정이 포함된 OU(조직 구성 단위)가 표시됩니다. 계정을 다른 OU로 이동하려면 Active Directory 사용자 및 컴퓨터를 사용해야 합니다.
    

    > [!NOTE]
    > Exchange Online에서는 이 확인란을 사용할 수 없습니다.



  - **사용자 지정 특성**   이 섹션에는 메일 사용자에 대해 정의된 사용자 지정 특성이 표시됩니다. 사용자 지정 특성 값을 지정하려면 **편집**![편집 아이콘](images/JJ218640.6f53ccb2-1f13-4c02-bea0-30690e6ea71d(EXCHG.150).gif "편집 아이콘")을 클릭합니다. 받는 사람에 대해 최대 15개의 사용자 지정 특성을 지정할 수 있습니다.

## 연락처 정보

**연락처 정보** 섹션을 사용하면 사용자의 연락처 정보를 보거나 변경할 수 있습니다. 이 페이지의 정보는 주소록에 표시됩니다. **기타 옵션**을 클릭하여 추가 상자를 표시합니다.


> [!TIP]
> <STRONG>시/도</STRONG> 상자를 사용하여 동적 메일 그룹, 전자 메일 주소 정책 또는 주소 목록에 대한 받는 사람 조건을 만들 수 있습니다.



## 조직

**조직** 섹션을 사용하면 조직에서의 사용자 역할에 대한 자세한 정보를 기록할 수 있습니다. 이 정보는 주소록에 표시됩니다. 또한 Outlook과 같은 전자 메일 클라이언트에서 액세스할 수 있는 가상 조직도를 만들 수 있습니다.

  - **직함**   이 상자에서 받는 사람의 직함을 보거나 변경합니다.

  - **부서**   이 상자에서 사용자가 근무하는 부서를 보거나 변경합니다. 이 상자를 사용하여 동적 메일 그룹, 전자 메일 주소 정책 또는 주소 목록에 대한 받는 사람 조건을 만들 수 있습니다.

  - **회사**   이 상자에서 사용자가 근무하는 회사를 보거나 변경합니다. 이 상자를 사용하여 동적 메일 그룹, 전자 메일 주소 정책 또는 주소 목록에 대한 받는 사람 조건을 만들 수 있습니다.

  - **관리자** 관리자를 추가하려면 **찾아보기**를 클릭합니다. **관리자 선택**에서 사람을 선택하고 **확인**을 클릭합니다.

  - **부하 직원**   이 입력란은 수정할 수 없습니다. *부하 직원*은 특정 관리자에게 보고하는 사용자입니다. 사용자에 대한 관리자를 지정한 경우 해당 사용자가 관리자 사서함의 세부 정보에 부하 직원으로 나타납니다. 예를 들어, Kari가 Chris와 Kate의 관리자이면 Chris와 Kate의 **관리자** 입력란에 Kari가 지정되고 Chris와 Kate는 Kari 계정 속성의 **부하 직원** 입력란에 표시됩니다.

## 전자 메일 주소

**전자 메일 주소** 섹션을 사용하면 메일 사용자와 연결된 전자 메일 주소를 보거나 변경할 수 있습니다. 여기에는 메일 사용자의 기본 SMTP 주소와 외부 전자 메일 주소 및 모든 관련 프록시 주소가 포함됩니다. 기본 SMTP 주소(*기본 회신 주소*)는 주소록에 굵게 표시되며 대문자로 된 **SMTP** 값이 **유형** 열에 표시됩니다. 기본적으로 메일 사용자가 만들어졌을 때 기본 SMTP 주소와 외부 전자 메일 주소는 동일합니다.

  - **추가**   이 사서함에 대해 새 전자 메일 주소를 추가하려면 **추가**![아이콘 추가](images/JJ218640.c1e75329-d6d7-4073-a27d-498590bbb558(EXCHG.150).gif "아이콘 추가")를 클릭합니다. 다음 주소 형식 중 하나를 선택합니다.
    
      - **SMTP**   기본 주소 유형입니다. 이 단추를 클릭하고 **\* 전자 메일 주소** 상자에 새 SMTP 주소를 입력합니다.
    
      - **사용자 지정 주소 유형**   이 단추를 클릭하고 **\* 전자 메일 주소** 상자에 지원되는 SMTP 이외의 전자 메일 주소 유형 중 하나를 입력합니다.
        

        > [!NOTE]
        > X.400 주소를 제외하고 Exchange는 사용자 지정 주소 형식이 올바른지 확인하지 않습니다. 지정하는 사용자 지정 주소는 해당 주소 유형에 대한 형식 요구 사항을 충족해야 합니다.



  - **외부 전자 메일 주소를 설정합니다.**   이 입력란을 사용하여 메일 사용자의 외부 주소를 변경합니다. 이 메일 사용자에게 보낸 전자 메일이 이 전자 메일 주소로 전달됩니다.

  - **이 받는 사람에게 적용된 전자 메일 주소 정책에 따라 전자 메일 주소를 자동으로 업데이트**   조직의 전자 메일 주소 정책에 대한 변경 내용에 따라 받는 사람의 전자 메일 주소가 자동으로 업데이트되도록 하려면 이 확인란을 선택합니다. 이 확인란은 기본적으로 선택되어 있습니다.
    

    > [!NOTE]
    > Exchange Online에서는 이 확인란을 사용할 수 없습니다.



## 메일 흐름 설정

**메일 흐름 설정** 섹션을 사용하여 다음 설정을 보거나 변경합니다.

  - **메시지 크기 제한**   이 설정은 메일 사용자가 보내고 받을 수 있는 메시지의 크기를 제어합니다. 보내고 받은 메시지의 최대 크기를 보고 변경하려면 **세부 정보 보기**를 클릭합니다.
    
      - **보낸 메시지**   이 사용자가 보내는 메시지의 최대 크기를 지정하려면 **최대 메시지 크기(KB)** 확인란을 선택하고 상자에 값을 입력합니다. 메시지 크기는 0KB에서 2,097,151KB 사이여야 합니다. 사용자가 지정된 크기보다 큰 메시지를 보내는 경우 해당 메시지는 설명이 포함된 오류 메시지와 함께 사용자에게 반환됩니다.
    
      - **받은 메시지**   이 사용자가 받는 메시지의 최대 크기를 지정하려면 **최대 메시지 크기(KB)** 확인란을 선택하고 상자에 값을 입력합니다. 메시지 크기는 0KB에서 2,097,151KB 사이여야 합니다. 지정된 크기보다 큰 메시지를 사용자에게 보내는 경우 해당 메시지는 설명이 포함된 오류 메시지와 함께 보낸 사람에게 반환됩니다.

  - **메시지 배달 제한**   이 설정은 메일 사용자에게 전자 메일 메시지를 보낼 수 있는 사용자를 제어합니다. 이러한 제한을 보고 변경하려면 **세부 정보 보기**를 클릭합니다.
    
      - **메시지 수락**   이 사용자에게 메시지를 보낼 수 있는 사용자를 지정할 수 있습니다.
        
          - **모든 보낸 사람**   사용자가 모든 보낸 사람이 보낸 메시지를 받을 수 있도록 지정하려면 이 옵션을 선택합니다. 여기에는 Exchange 조직의 보낸 사람과 외부 보낸 사람이 모두 포함됩니다. 기본적으로 이 옵션이 선택됩니다. 이 옵션은 **보낸 사람 모두 인증 필요** 확인란의 선택을 취소할 경우에만 외부 사용자를 포함합니다. 이 확인란을 선택하면 외부 사용자가 보낸 메시지가 거부됩니다.
        
          - **다음 목록에 있는 보낸 사람만**   Exchange 조직에서 지정된 보낸 사람이 보낸 메시지만 사용자가 받을 수 있도록 지정하려면 이 옵션을 선택합니다. **추가**![아이콘 추가](images/JJ218640.c1e75329-d6d7-4073-a27d-498590bbb558(EXCHG.150).gif "아이콘 추가")를 클릭하여 **받는 사람 선택** 페이지를 표시합니다. 이 페이지에는 Exchange 조직의 모든 받는 사람 목록이 표시됩니다. 원하는 받는 사람을 선택하여 목록에 추가한 다음 **확인**을 클릭합니다. 또한 검색 상자에 받는 사람 이름을 입력한 다음 **검색**![검색 아이콘](images/Dd353189.773574d0-9b92-4cab-9f6b-81532c7418b9(EXCHG.150).gif "검색 아이콘")을 클릭하여 특정 받는 사람을 검색할 수도 있습니다.
        
          - **보낸 사람 모두 인증 필요**   익명 사용자가 사용자에 메시지를 보낼 수 없도록 하려면 이 옵션을 선택합니다.
    
      - **다음 사람이 보낸 메시지 거부**   이 사용자에게 메시지를 보내지 못하도록 차단할 수 있습니다.
        
          - **보낸 사람 없음**   Exchange 조직의 모든 보낸 사람이 보낸 메시지를 사서함에서 거부하지 않도록 지정하려면 이 옵션을 선택합니다. 기본적으로 이 옵션이 선택됩니다.
        
          - **다음 목록에 있는 보낸 사람**   Exchange 조직에서 지정된 보낸 사람이 보낸 메시지를 사서함에서 거부하도록 지정하려면 이 옵션을 선택합니다. **추가**![아이콘 추가](images/JJ218640.c1e75329-d6d7-4073-a27d-498590bbb558(EXCHG.150).gif "아이콘 추가")를 클릭하여 **받는 사람 선택** 페이지를 표시합니다. 이 페이지에는 Exchange 조직의 모든 받는 사람 목록이 표시됩니다. 원하는 받는 사람을 선택하여 목록에 추가한 다음 **확인**을 클릭합니다. 또한 검색 상자에 받는 사람 이름을 입력한 다음 **검색**![검색 아이콘](images/Dd353189.773574d0-9b92-4cab-9f6b-81532c7418b9(EXCHG.150).gif "검색 아이콘")을 클릭하여 특정 받는 사람을 검색할 수도 있습니다.

## 소속 그룹

**소속 그룹** 섹션을 사용하면 이 사용자가 속해 있는 메일 그룹 또는 보안 그룹의 목록을 볼 수 있습니다. 이 페이지에서는 구성원 정보를 변경할 수 없습니다. 사용자가 조직에 있는 하나 이상의 동적 메일 그룹에 대한 기준에 일치할 수 있습니다. 그러나 동적 메일 그룹은 사용될 때마다 해당 구성원이 계산되므로 이 페이지에 표시되지 않습니다.

## 메일 설명

**메일 설명** 섹션에서는 메일 설명을 추가하여 이 받는 사람에게 메시지를 보낼 경우 발생할 수 있는 문제를 사용자에게 알릴 수 있습니다. 메일 설명은 새 전자 메일 메시지의 받는 사람, 참조 또는 숨은 참조 필드에 이 받는 사람이 추가될 때 정보 표시줄에 표시되는 텍스트입니다.


> [!NOTE]
> 메일 설명은 HTML 태그를 포함할 수 있지만 스크립트는 사용할 수 없습니다. 표시되는 사용자 지정 메일 설명의 길이는 175자를 초과할 수 없습니다. 단, HTML 태그는 길이 제한 계산에 포함되지 않습니다.



## 셸을 사용하여 메일 사용자 속성 변경

메일 사용자에 대한 속성은 Active Directory와 Exchange 둘 다에 저장됩니다. 일반적으로 조직 및 연락처 정보 속성을 보거나 변경하려면 **Get-User** 및 **Set-User** cmdlet을 사용합니다. 전자 메일 주소, 메일 설명, 사용자 지정 특성 및 메일 사용자를 주소 목록에서 숨길지 여부 등, 메일 관련 속성을 보거나 변경하려면 **Get-MailUser** 및 **Set-MailUser** cmdlet을 사용합니다.

메일 사용자의 속성을 보거나 변경하려면 **Get-MailUser** 및 **Set-MailUser** cmdlet을 사용합니다. 자세한 내용은 다음 항목을 참조하십시오.

  - [Get-User](https://technet.microsoft.com/ko-kr/library/aa996896\(v=exchg.150\))

  - [Set-User](https://technet.microsoft.com/ko-kr/library/aa998221\(v=exchg.150\))

  - [Get-MailUser](https://technet.microsoft.com/ko-kr/library/aa997254\(v=exchg.150\))

  - [Set-MailUser](https://technet.microsoft.com/ko-kr/library/aa995971\(v=exchg.150\))

다음은 셸을 사용하여 메일 사용자 속성을 변경하는 예입니다.

다음 예에서는 Pilar Pinilla의 외부 전자 메일 주소를 설정합니다.

    Set-MailUser "Pilar Pinilla" -ExternalEmailAddress pilarp@tailspintoys.com

다음 예에서는 조직의 주소록에서 모든 메일 사용자를 숨깁니다.

    Get-MailUser | Set-MailUser -HiddenFromAddressListsEnabled $true

다음 예에서는 모든 메일 사용자의 Company 속성을 Contoso로 설정합니다.

    Get-User -ResultSize unlimited -Filter {(RecipientTypeDetails -eq 'mailuser')} | Set-User -Company Contoso

이 예에서는 Company 속성이 Contoso로 설정된 모든 메일 사용자에 대해 CustomAttribute1 속성을 ContosoEmployee로 설정합니다.

    Get-User -ResultSize unlimited -Filter {(RecipientTypeDetails -eq 'mailuser') -and (Company -eq 'Contoso')}| Set-MailUser -CustomAttribute1 ContosoEmployee

## 작동 여부는 어떻게 확인합니까?

메일 사용자에 대한 속성이 변경되었는지 확인하려면 다음을 수행하십시오.

  - EAC에서 메일 사용자를 선택한 다음 **편집**![편집 아이콘](images/JJ218640.6f53ccb2-1f13-4c02-bea0-30690e6ea71d(EXCHG.150).gif "편집 아이콘")을 클릭하여 변경한 속성을 봅니다.

  - 셸에서 **Get-User** 및 **Get-MailUser** cmdlet을 사용하여 변경 사항을 확인합니다. 셸을 사용할 때 얻을 수 있는 한 가지 이점은 여러 메일 연락처의 여러 속성을 볼 수 있다는 것입니다.
    
        Get-MailUser | Fl Name,CustomAttribute1 
    
    모든 메일 연락처에 대한 Company 속성이 Contoso로 설정된 위의 예에서 변경 사항을 확인하려면 다음 명령을 실행합니다.
    
        Get-User -ResultSize unlimited -Filter {(RecipientTypeDetails -eq 'mailuser')} | FL Name,Company
    
    모든 메일 사용자의 CustomAttribute1 속성이 ContosoEmployee로 설정된 위의 예에서 변경 사항을 확인하려면 다음 명령을 실행합니다.
    
        Get-MailUser | Fl Name,CustomAttribute1 

## 메일 사용자 일괄 편집

또한 EAC를 사용하여 여러 메일 사용자에 대한 선택된 속성을 변경할 수 있습니다. EAC의 연락처 목록에서 두 명 이상의 메일 사용자를 선택하면 일괄 편집이 가능한 속성이 세부 정보 창에 표시됩니다. 이러한 속성 중 하나를 변경하면 변경 내용이 선택된 모든 받는 사람에게 적용됩니다.

메일 사용자를 일괄 편집할 때 다음 속성 영역을 변경할 수 있습니다.

  - **연락처 정보**   주소, 우편 번호 및 구/군/시 이름과 같은 공유 속성을 변경합니다.

  - **조직**   부서 이름, 회사 이름 및 선택한 메일 연락처나 메일 사용자가 보고하는 관리자 등의 공유 속성을 변경합니다.

## EAC를 사용하여 메일 사용자 일괄 편집

1.  EAC에서 **받는 사람** \> **연락처**로 이동합니다.

2.  연락처 목록에서 두 명 이상의 메일 사용자를 선택합니다. 메일 연락처 및 메일 사용자의 조합을 대량으로 편집할 수 없습니다.
    

    > [!TIP]
    > Shift 키를 누른 상태로 편집할 첫 번째 메일 사용자를 클릭한 다음 마지막 메일 사용자를 클릭하면 인접한 여러 명의 메일 사용자를 한꺼번에 선택할 수 있습니다. 또한 Ctrl 키를 누른 상태로 편집할 각 메일 사용자를 클릭하여 여러 메일 사용자를 선택할 수도 있습니다.



3.  세부 정보 창의 **대량 편집**에서 **연락처** 또는 **조직** 아래의 **업데이트**를 클릭합니다.

4.  속성 페이지에서 필요한 사항을 변경하고 변경 내용을 저장합니다.

## 작동 여부는 어떻게 확인합니까?

메일 사용자가 일괄 편집되었는지 확인하려면 다음 중 하나를 수행합니다.

  - EAC에서 일괄 편집한 각각의 메일 사용자를 선택한 다음 **편집**![편집 아이콘](images/JJ218640.6f53ccb2-1f13-4c02-bea0-30690e6ea71d(EXCHG.150).gif "편집 아이콘")을 클릭하여 변경한 속성을 봅니다.

  - 셸에서 **Get-User** cmdlet을 사용하여 변경 사항을 확인합니다. 예를 들어, EAC에서 일괄 편집 기능을 사용하여 A. Datum Corporation이라는 공급업체의 모든 메일 사용자에 대해 관리자와 사무실을 변경한 경우 이러한 변경 내용을 확인하려면 셸에서 다음 명령을 실행할 수 있습니다.
    
        Get-User -ResultSize unlimited -Filter {(RecipientTypeDetails -eq 'mailuser') -and (Company -eq 'Adatum')} | fl Name,Office,Manager

## 디렉터리 동기화를 사용 하 여 Exchange Online의 메일 사용자를 관리 하려면

이 섹션에서는 Exchange Online에서 디렉터리 동기화를 사용 하 여 메일 사용자를 관리 하는 방법에 대 한 정보를 제공 합니다. 디렉터리 동기화 온-프레미스 및 클라우드 호스팅 사서함을 사용 하 여 하이브리드 고객을 위해 사용할 수 있으며 완벽 하 게 호스팅된 Exchange Online 고객을 위한 해당 Active Directory가 온-프레미스.


> [!NOTE]
> 디렉터리 동기화를 사용하여 받는 사람을 관리하는 경우 Office 365 관리 센터에서 계속해서 사용자를 추가하고 관리할 수 있습니다. 하지만 이러한 받는 사람은 온-프레미스 Active Directory와 동기화되지는 않습니다. 디렉터리 동기화는 온-프레미스 Active Directory의 받는 사람만 클라우드로 동기화하기 때문입니다.




> [!NOTE]
> 다음 기능을 사용하려면 디렉터리 동기화를 사용하는 것이 좋습니다. 
> <UL>
> <LI>
> <P><STRONG>Outlook의 수신 허용-보낸사람 및 수신된 거부 목록</STRONG> 서비스에 동기화 할 때 이러한 목록을 우선 스팸 필터링 서비스. 그러면 사용자가 자신의 수신 허용-보낸사람 및 수신된 거부 목록 사용자별 또는 도메인당 기준를 관리할 수 있습니다.</P>
> <LI>
> <P><STRONG>디렉터리 기반 Edge 차단 (DBEB)</STRONG> DBEB에 대 한 자세한 내용은 <A href="https://technet.microsoft.com/ko-kr/library/dn600322(v=exchg.150)">디렉터리 기반 Edge 차단을 사용하여 잘못된 받는 사람에게 전송된 메시지 거부</A>을 참조 하십시오.</P>
> <LI>
> <P><STRONG>최종 사용자 스팸 격리</STRONG> 최종 사용자 스팸 격리에 액세스 하기 위해 유효한 Office 365 사용자 ID와 암호를 최종 사용자가 있어야 합니다. 온-프레미스 사서함이 있는 고객 유효한 전자 메일 사용자 여야 합니다.</P>
> <LI>
> <P><STRONG>전송 규칙</STRONG> 디렉터리 동기화를 사용 하면 기존 Active Directory 사용자 및 그룹을 사용 하 여 클라우드 자동으로 업로드 있으며 만들 수 있습니다 다음 전송 규칙 백업/복원 시 해당 대상 특정 사용자 또는 그룹 EAC 또는 원격 Windows PowerShell을 통해이 수동으로 추가 하지 않고도 합니다. Note 디렉터리 동기화를 통해 해당 <A href="https://go.microsoft.com/fwlink/?linkid=507569">동적 메일 그룹</A> 을 동기화 할 수 없습니다.</P></LI></UL>



**시작하기 전에**

필요한 사용 권한을 얻고 [디렉터리 동기화 준비](https://go.microsoft.com/fwlink/p/?linkid=308908)의 설명에 따라 디렉터리 동기화를 위한 준비 합니다.

사용자 디렉터리를 동기화하려면

1.  [디렉터리 동기화 활성화](https://go.microsoft.com/fwlink/p/?linkid=308909)의 설명에 따라 디렉터리 동기화를 활성화 합니다.

2.  [디렉터리 동기화 컴퓨터 설정](http://go.microsoft.com/fwlink/p/?linkid=308911)의 설명에 따라 디렉터리 동기화 컴퓨터를 설정합니다.

3.  [구성 마법사를 사용하여 디렉터리 동기화](http://go.microsoft.com/fwlink/?linkid=308912)의 설명에 따라 디렉터리를 동기화합니다.
    

    > [!IMPORTANT]
    > Azure Active Directory 동기화 도구 구성 마법사를 완료하면 Active Directory 포리스트에 <STRONG>MSOL_AD_SYNC</STRONG> 계정이 만들어집니다. 이 계정을 사용하여 온-프레미스 Active Directory 정보를 읽고 동기화합니다. 디렉터리 동기화가 정상적으로 작동하도록 하려면 로컬 디렉터리 동기화 서버의 TCP 443이 열려 있는지 확인합니다.



4.  [동기화된 사용자 활성화](http://go.microsoft.com/fwlink/p/?linkid=308913)의 설명에 따라 동기화된 사용자를 활성화합니다.

5.  [디렉터리 동기화 관리](http://go.microsoft.com/fwlink/p/?linkid=308915)의 설명에 따라 디렉터리 동기화를 관리합니다.

6.  Exchange Online가 올바르게 동기화를 확인 합니다. EAC에서 **받는 사람** 에 게 이동 \> **연락처** 및 온-프레미스 환경에서 사용자의 목록을 동기화 할 올바르게 보기입니다.
