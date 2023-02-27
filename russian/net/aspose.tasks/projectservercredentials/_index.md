---
title: Class ProjectServerCredentials
second_title: Справочник по Aspose.Tasks для .NET API
description: Aspose.Tasks.ProjectServerCredentials сорт. Учетные данные используемые для подключения к Project Online или локальному экземпляру Project Server.
type: docs
weight: 1240
url: /ru/net/aspose.tasks/projectservercredentials/
---
## ProjectServerCredentials class

Учетные данные, используемые для подключения к Project Online или локальному экземпляру Project Server.

```csharp
public sealed class ProjectServerCredentials
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ProjectServerCredentials](projectservercredentials/#constructor)(string, NetworkCredential) | Инициализирует новый экземпляр`ProjectServerCredentials` class с использованием URL-адреса конечной точки Project Web Access и сетевых учетных данных. |
| [ProjectServerCredentials](projectservercredentials/#constructor_1)(string, string) | Инициализирует новый экземпляр`ProjectServerCredentials` класс, использующий URL-адрес сайта SharePoint и действительный токен авторизации SPOYDCRL для сайта SharePoint PWA (Project Web Access). |
| [ProjectServerCredentials](projectservercredentials/#constructor_2)(string, string, string) | Инициализирует новый экземпляр`ProjectServerCredentials` класс, используя URL-адрес сайта SharePoint, имя пользователя и пароль. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [AuthToken](../../aspose.tasks/projectservercredentials/authtoken/) { get; } | Получает токен авторизации для экземпляра SharePoint. |
| [SiteUrl](../../aspose.tasks/projectservercredentials/siteurl/) { get; } | Получает URL-адрес PWA на сайте SharePoint или URL-адрес локального сервера Project Server. Например, https://your_company_name.sharepoint.com/sites/pwa"; |
| [UserName](../../aspose.tasks/projectservercredentials/username/) { get; } | Получает имя пользователя для сайта SharePoint. |

## Методы

| Имя | Описание |
| --- | --- |
| override [ToString](../../aspose.tasks/projectservercredentials/tostring/)() | Возвращает строковое представление этого экземпляра. |

### Смотрите также

* пространство имен [Aspose.Tasks](../../aspose.tasks/)
* сборка [Aspose.Tasks](../../)


