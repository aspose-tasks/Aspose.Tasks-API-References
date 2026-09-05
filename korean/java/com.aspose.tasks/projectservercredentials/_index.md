---
title: "ProjectServerCredentials"
second_title: "Aspose.Tasks for Java API Reference"
description: "Project Online 또는 온프레미스 Project Server 인스턴스에 연결하는 데 사용되는 자격 증명입니다."
type: docs
weight: 225
url: /ko/java/com.aspose.tasks/projectservercredentials/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerCredentials
```

Project Online 또는 온프레미스 Project Server 인스턴스에 연결하는 데 사용되는 자격 증명입니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ProjectServerCredentials(String siteUrl, String authToken)](#ProjectServerCredentials-java.lang.String-java.lang.String-) | SharePoint 사이트의 URL과 SharePoint의 PWA(프로젝트 웹 액세스) 사이트에 대한 유효한 SPOIDCRL 인증 토큰을 사용하여 [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) 클래스의 새 인스턴스를 초기화합니다. |
| [ProjectServerCredentials(String siteUrl, String userName, String password)](#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-) | SharePoint 사이트의 URL, 사용자 이름 및 비밀번호를 사용하여 [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getAuthToken()](#getAuthToken--) | SharePoint 인스턴스에 대한 인증 토큰을 가져옵니다. |
| [getSiteUrl()](#getSiteUrl--) | SharePoint 사이트의 PWA URL 또는 온프레미스 Project Server의 URL을 가져옵니다. |
| [getUserName()](#getUserName--) | SharePoint 사이트의 사용자 이름을 가져옵니다. |
| [toString()](#toString--) | 이 인스턴스의 문자열 표현을 반환합니다. |
### ProjectServerCredentials(String siteUrl, String authToken) {#ProjectServerCredentials-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String authToken)
```


SharePoint 사이트의 URL과 SharePoint의 PWA(프로젝트 웹 액세스) 사이트에 대한 유효한 SPOIDCRL 인증 토큰을 사용하여 [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| siteUrl | java.lang.String | Project Online의 PWA (Project Web Access) API URL입니다. |
|  | authToken | java.lang.String | SharePoint의 PWA (Project Web Access) 사이트에 대한 인증 토큰 (SPOIDCRL)입니다. |

--------------------

SharePoint Online 사이트에 대한 AuthToken이 이미 있는 경우 이 생성자를 사용하여 ProjectOnline에 연결합니다. |

### ProjectServerCredentials(String siteUrl, String userName, String password) {#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String userName, String password)
```


SharePoint 사이트의 URL, 사용자 이름 및 비밀번호를 사용하여 [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| siteUrl | java.lang.String | Project Online의 PWA (Project Web Access) API URL입니다. |
| userName | java.lang.String | SharePoint 사이트의 사용자 이름입니다. |
|  | password | java.lang.String | SharePoint 사이트의 비밀번호입니다. |

--------------------

이 생성자를 사용하여 ProjectOnline에 연결합니다. 레거시 인증은 Azure 포털 및 Office 365 관리 센터에서 활성화되어야 함을 유의하십시오. |

### getAuthToken() {#getAuthToken--}
```
public final String getAuthToken()
```


SharePoint 인스턴스에 대한 인증 토큰을 가져옵니다.

**Returns:**
java.lang.String - SharePoint 인스턴스에 대한 인증 토큰입니다.
### getSiteUrl() {#getSiteUrl--}
```
public final String getSiteUrl()
```


SharePoint 사이트의 PWA URL 또는 온프레미스 Project Server URL을 가져옵니다. 예: https://your\_company\_name.sharepoint.com/sites/pwa\";

**Returns:**
java.lang.String - SharePoint 사이트의 PWA URL 또는 온프레미스 Project Server URL입니다.
### getUserName() {#getUserName--}
```
public final String getUserName()
```


SharePoint 사이트의 사용자 이름을 가져옵니다.

**Returns:**
java.lang.String - SharePoint 사이트의 사용자 이름입니다.
### toString() {#toString--}
```
public String toString()
```


이 인스턴스의 문자열 표현을 반환합니다.

**Returns:**
java.lang.String - 이 인스턴스의 문자열 표현입니다.
