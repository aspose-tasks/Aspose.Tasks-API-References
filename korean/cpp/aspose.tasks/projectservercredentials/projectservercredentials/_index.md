---
title: "Aspose::Tasks::ProjectServerCredentials::ProjectServerCredentials 생성자"
linktitle: "ProjectServerCredentials"
articleTitle: "ProjectServerCredentials"
second_title: "C++용 Aspose.Tasks"
description: "ProjectServerCredentials 클래스의 새 인스턴스를 SharePoint 사이트 URL과 SharePoint의 PWA(프로젝트 웹 액세스)를 위한 유효한 SPOIDCRL 인증 토큰을 사용하여 초기화합니다 ( Proj"
type: docs
weight: 10
url: /ko/cpp/aspose.tasks/projectservercredentials/projectservercredentials/
---

## ProjectServerCredentials (1 of 3) {#projectservercredentials_1}

SharePoint 사이트 URL과 SharePoint의 PWA(프로젝트 웹 액세스) 사이트에 대한 유효한 SPOIDCRL 인증 토큰을 사용하여 ProjectServerCredentials 클래스의 새 인스턴스를 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & authToken)
```

| 매개변수 | 설명 |
| --- | --- |
| siteUrl | Project Online의 PWA(프로젝트 웹 액세스) API URL입니다. |
| authToken | SharePoint의 PWA(프로젝트 웹 액세스) 사이트에 대한 인증 토큰(SPOIDCRL)입니다. |

---

## ProjectServerCredentials (2 of 3) {#projectservercredentials_2}

ProjectServerCredentials 클래스의 새 인스턴스를 SharePoint 사이트 URL, 사용자 이름 및 비밀번호를 사용하여 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & userName, const System::String & password)
```

| 매개변수 | 설명 |
| --- | --- |
| siteUrl | Project Online의 PWA(프로젝트 웹 액세스) API URL입니다. |
| userName | SharePoint 사이트의 사용자 이름입니다. |
| password | SharePoint 사이트의 비밀번호입니다. |

---

## ProjectServerCredentials (3 of 3) {#projectservercredentials_3}

ProjectServerCredentials 클래스의 새 인스턴스를 Project Web Access 엔드포인트 URL 및 네트워크 자격 증명을 사용하여 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::SharedPtr< System::Net::NetworkCredential > & credentials)
```

| 매개변수 | 설명 |
| --- | --- |
| siteUrl | Project Web Access 엔드포인트의 URL입니다. |
| credentials | Project Web Access 엔드포인트에 로그인하는 데 사용되는 자격 증명입니다. |

