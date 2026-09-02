---
title: "منشئ Aspose::Tasks::ProjectServerCredentials::ProjectServerCredentials"
linktitle: "ProjectServerCredentials"
articleTitle: "ProjectServerCredentials"
second_title: "Aspose.Tasks لـ C++"
description: "يُهيئ مثلاً جديداً من فئة ProjectServerCredentials باستخدام عنوان URL لموقع SharePoint ورمز تفويض SPOIDCRL صالح لـ PWA (Proj"
type: docs
weight: 10
url: /ar/cpp/aspose.tasks/projectservercredentials/projectservercredentials/
---

## ProjectServerCredentials (1 of 3) {#projectservercredentials_1}

ينشئ نسخة جديدة من فئة ProjectServerCredentials باستخدام عنوان URL لموقع SharePoint ورمز تفويض SPOIDCRL صالح لموقع PWA (Project Web Access) الخاص بـ SharePoint.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & authToken)
```

| معامل | الوصف |
| --- | --- |
| siteUrl | عنوان URL لـ PWA (Project Web Access) API الخاص بـ Project Online. |
| authToken | رمز التفويض (SPOIDCRL) لموقع PWA (Project Web Access) الخاص بـ SharePoint. |

---

## ProjectServerCredentials (2 of 3) {#projectservercredentials_2}

يُهيئ مثلاً جديداً من فئة ProjectServerCredentials باستخدام عنوان URL لموقع SharePoint، اسم المستخدم وكلمة المرور.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & userName, const System::String & password)
```

| معامل | الوصف |
| --- | --- |
| siteUrl | عنوان URL لـ PWA (Project Web Access) API الخاص بـ Project Online. |
| userName | اسم المستخدم لموقع SharePoint. |
| password | كلمة المرور لموقع SharePoint. |

---

## ProjectServerCredentials (3 of 3) {#projectservercredentials_3}

يُهيئ مثلاً جديداً من فئة ProjectServerCredentials باستخدام عنوان URL لنقطة النهاية Project Web Access وبيانات الاعتماد الشبكية.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::SharedPtr< System::Net::NetworkCredential > & credentials)
```

| معامل | الوصف |
| --- | --- |
| siteUrl | عنوان URL لنقطة النهاية Project Web Access. |
| بيانات الاعتماد | بيانات الاعتماد المستخدمة لتسجيل الدخول إلى نقطة النهاية Project Web Access. |

