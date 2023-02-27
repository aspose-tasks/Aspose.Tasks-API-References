---
title: ProjectServerCredentials.ProjectServerCredentials
second_title: Справочник по Aspose.Tasks для .NET API
description: ProjectServerCredentials строитель. Инициализирует новый экземплярProjectServerCredentials класс использующий URLадрес сайта SharePoint и действительный токен авторизации SPOYDCRL для сайта SharePoint PWA Project Web Access.
type: docs
weight: 10
url: /ru/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

Инициализирует новый экземпляр[`ProjectServerCredentials`](../) класс, использующий URL-адрес сайта SharePoint и действительный токен авторизации SPOYDCRL для сайта SharePoint PWA (Project Web Access).

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| siteUrl | String | URL-адрес API PWA (Project Web Access) Project Online. |
| authToken | String | Маркер авторизации (SPOYDCRL) для сайта SharePoint PWA (Project Web Access). |

### Примечания

Используйте этот конструктор для подключения к ProjectOnline, если у вас уже есть AuthToken для вашего сайта SharePoint Online.

### Смотрите также

* class [ProjectServerCredentials](../)
* пространство имен [Aspose.Tasks](../../projectservercredentials/)
* сборка [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

Инициализирует новый экземпляр[`ProjectServerCredentials`](../) класс, используя URL-адрес сайта SharePoint, имя пользователя и пароль.

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| siteUrl | String | URL-адрес API PWA (Project Web Access) Project Online. |
| userName | String | Имя пользователя для сайта SharePoint. |
| password | String | Пароль для сайта SharePoint. |

### Примечания

Используйте этот конструктор для подключения к ProjectOnline. Обратите внимание, что устаревшая проверка подлинности должна быть включена на портале Azure и в центре администрирования Office 365.

### Смотрите также

* class [ProjectServerCredentials](../)
* пространство имен [Aspose.Tasks](../../projectservercredentials/)
* сборка [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

Инициализирует новый экземпляр[`ProjectServerCredentials`](../) class с использованием URL-адреса конечной точки Project Web Access и сетевых учетных данных.

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| siteUrl | String | URL-адрес конечной точки веб-доступа к проекту. |
| credentials | NetworkCredential | Учетные данные, используемые для входа в конечную точку Project Web Access. |

### Примечания

Используйте этот конструктор для подключения к локальному экземпляру Project Server через PWA.

### Примеры

В этом примере экземпляр[`ProjectServerManager`](../../projectservermanager/)Класс используется для чтения списка проектов из экземпляра Project Server, расположенного по адресу http://project_server_instance.local .

```csharp
string site = "http://project_server_instance.local/sites/pwa";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);

var list = manager.GetProjectList();
foreach (var projectInfo in list)
{
    Console.WriteLine("{0} - {1} - {2}", projectInfo.Id, projectInfo.CreatedDate, projectInfo.Name);
}
```

### Смотрите также

* class [ProjectServerCredentials](../)
* пространство имен [Aspose.Tasks](../../projectservercredentials/)
* сборка [Aspose.Tasks](../../../)


