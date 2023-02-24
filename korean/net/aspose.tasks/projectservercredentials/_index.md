---
title: ProjectServerCredentials
second_title: .NET API 참조용 Aspose.Tasks
description: Project Online 또는 Project Server의 온프레미스 인스턴스에 연결하는 데 사용되는 자격 증명.
type: docs
weight: 1240
url: /ko/net/aspose.tasks/projectservercredentials/
---
## ProjectServerCredentials class

Project Online 또는 Project Server의 온-프레미스 인스턴스에 연결하는 데 사용되는 자격 증명.

```csharp
public sealed class ProjectServerCredentials
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [ProjectServerCredentials](projectservercredentials/#constructor)(string, NetworkCredential) | 의 새 인스턴스를 초기화합니다.`ProjectServerCredentials` Project Web Access 끝점 및 네트워크 자격 증명의 URL을 사용하는 클래스. |
| [ProjectServerCredentials](projectservercredentials/#constructor_1)(string, string) | 의 새 인스턴스를 초기화합니다.`ProjectServerCredentials` SharePoint 사이트의 URL과 SharePoint의 PWA(Project Web Access) 사이트에 대한 유효한 SPOIDCRL 인증 토큰을 사용하는 클래스. |
| [ProjectServerCredentials](projectservercredentials/#constructor_2)(string, string, string) | 의 새 인스턴스를 초기화합니다.`ProjectServerCredentials` SharePoint 사이트의 URL, 사용자 이름 및 암호를 사용하는 클래스. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [AuthToken](../../aspose.tasks/projectservercredentials/authtoken/) { get; } | SharePoint 인스턴스에 대한 인증 토큰을 가져옵니다. |
| [SiteUrl](../../aspose.tasks/projectservercredentials/siteurl/) { get; } | SharePoint 사이트에서 PWA의 URL 또는 온-프레미스 Project Server의 URL을 가져옵니다. 예: https://your_company_name.sharepoint.com/sites/pwa"; |
| [UserName](../../aspose.tasks/projectservercredentials/username/) { get; } | SharePoint 사이트의 사용자 이름을 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| override [ToString](../../aspose.tasks/projectservercredentials/tostring/)() | 이 인스턴스의 문자열 표현을 반환합니다. |

### 또한보십시오

* 네임스페이스 [Aspose.Tasks](../../aspose.tasks/)
* 집회 [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->