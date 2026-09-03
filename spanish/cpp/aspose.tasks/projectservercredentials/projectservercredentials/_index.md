---
title: "Aspose::Tasks::ProjectServerCredentials::ProjectServerCredentials constructor"
linktitle: "ProjectServerCredentials"
articleTitle: "ProjectServerCredentials"
second_title: "Aspose.Tasks for C++"
description: "Inicializa una nueva instancia de la clase ProjectServerCredentials usando la URL del sitio SharePoint y un token de autorización SPOIDCRL válido para el PWA ( Project Web Access) de SharePoint."
type: docs
weight: 10
url: /es/cpp/aspose.tasks/projectservercredentials/projectservercredentials/
---

## ProjectServerCredentials (1 of 3) {#projectservercredentials_1}

Inicializa una nueva instancia de la clase ProjectServerCredentials usando la URL del sitio SharePoint y un token de autorización SPOIDCRL válido para el sitio PWA (Project Web Access) de SharePoint.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & authToken)
```

| Parámetro | Descripción |
| --- | --- |
| siteUrl | La URL del API PWA ( Project Web Access) de Project Online. |
| authToken | El token de autorización (SPOIDCRL) para el sitio PWA ( Project Web Access) de SharePoint. |

---

## ProjectServerCredentials (2 of 3) {#projectservercredentials_2}

Inicializa una nueva instancia de la clase ProjectServerCredentials usando la URL del sitio SharePoint, nombre de usuario y contraseña.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & userName, const System::String & password)
```

| Parámetro | Descripción |
| --- | --- |
| siteUrl | La URL del API PWA ( Project Web Access) de Project Online. |
| userName | El nombre de usuario para el sitio SharePoint. |
| password | La contraseña para el sitio SharePoint. |

---

## ProjectServerCredentials (3 of 3) {#projectservercredentials_3}

Inicializa una nueva instancia de la clase ProjectServerCredentials usando la URL del punto de enlace Project Web Access y credenciales de red.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::SharedPtr< System::Net::NetworkCredential > & credentials)
```

| Parámetro | Descripción |
| --- | --- |
| siteUrl | La URL del punto de enlace de Project Web Access. |
| credenciales | Las credenciales usadas para iniciar sesión en el punto de enlace de Project Web Access. |

