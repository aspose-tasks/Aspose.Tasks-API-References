---
title: "Project.Project"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ Project. يهيئ نسخة جديدة من فئة Project."
type: docs
weight: 10
url: /ar/net/aspose.tasks/project/project/
---
## Project() {#constructor}

يهيئ نسخة جديدة من فئة [`Project`](../).

```csharp
public Project()
```

## الأمثلة

يعرض كيفية إنشاء مشروع وحفظه بتنسيق MPP دون تمرير ملف قالب MPP.

```csharp
var project = new Project();

// سيتم حفظ المشروع بتنسيق MPP باستخدام قالب MPP الداخلي.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, string) {#constructor_12}

يهيئ نسخة جديدة من فئة [`Project`](../) من قالب محمي بكلمة مرور (ملف mpp أو mpt موجود).

```csharp
public Project(string projectTemplate, string protectionPassword)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| projectTemplate | سلسلة | المسار إلى القالب لإنشاء المشروع منه. |
| protectionPassword | سلسلة | كلمة مرور الحماية. |

## ملاحظات

قراءة الملفات المحمية بكلمة مرور مدعومة حاليًا لتنسيق ملف MSP 2003 فقط.

## الأمثلة

يعرض كيفية قراءة ملفات MPP المحمية بكلمة مرور.

```csharp
var project = new Project(DataDir + "PasswordProtectedProject.mpp", "password");
Console.WriteLine(project.Get(Prj.Name));
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string) {#constructor_8}

يهيئ نسخة جديدة من فئة [`Project`](../) من قالب (ملف mpp أو mpt موجود).

```csharp
public Project(string projectTemplate)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| projectTemplate | سلسلة | المسار إلى القالب لإنشاء المشروع منه. |

## الأمثلة

يعرض كيفية قراءة ملف MPP.

```csharp
var project = new Project(DataDir + "ReadProjectFiles.mpp");
project.Save(OutDir + "ReadProjectFiles_out.mpp", SaveFileFormat.Xml);
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, PrimaveraReadOptions) {#constructor_5}

يهيئ نسخة جديدة من فئة [`Project`](../) من الدفق مع النسخة المحددة من فئة [`PrimaveraReadOptions`](../../primaverareadoptions/).

```csharp
public Project(Stream stream, PrimaveraReadOptions options)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| دفق | دفق | دفق فئة المشروع Streamclass |
| options | PrimaveraReadOptions | الكائن المحدد من فئة [`PrimaveraReadOptions`](../../primaverareadoptions/) الذي يسمح بتخصيص قراءة صيغ Primavera (XER أو XML). |

## الأمثلة

يوضح كيفية قراءة مشروع من دفق باستخدام ملف Primavera XML أو Primavera XER يحتوي على عدة مشاريع.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open, FileAccess.Read))
{
    // يعيد مشروعًا بمعرف UID خاص.
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### انظر أيضًا

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, ParseErrorCallback) {#constructor_10}

يهيئ نسخة جديدة من فئة [`Project`](../) من قالب (ملف mpp أو mpt موجود).

```csharp
public Project(string projectTemplate, ParseErrorCallback parseErrorHandler)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| projectTemplate | سلسلة | المسار إلى القالب لإنشاء المشروع منه. |
| parseErrorHandler | ParseErrorCallback | طريقة الاستدعاء المحددة لمعالجة أخطاء تحليل XML. |

## الأمثلة

يوضح كيفية قراءة مشروع من تدفق يحتوي على ملف XML بأحرف غير صالحة.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // افتح الملف الذي يحتوي على XML مع فترات زمنية مكسورة
    var project = new Project(pathToModifiedXml, CustomDurationHandlerForFile2);
    Console.WriteLine(project.Get(Prj.Name));
}

public static object CustomDurationHandlerForFile2(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Console.WriteLine("Object field: {0}, Object field type: {1}, Invalid value: {2}", args.FieldName, args.FieldType, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var newValue = Duration.ParseTimeSpan(duration);
    Console.WriteLine("New value : {0}", newValue);
    return newValue;
}
```

### انظر أيضًا

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream) {#constructor_2}

ينشئ كائنًا جديدًا من فئة [`Project`](../) من دفق.

```csharp
public Project(Stream stream)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| دفق | دفق | دفق لتحميل القالب منه. |

## الأمثلة

يوضح كيفية قراءة ملف مشروع XML من دفق.

```csharp
using (Stream stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var project = new Project(stream);
    project.Save(OutDir + "ReadProjectFileFromStream_out.xml", SaveFileFormat.Xml);
}
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(StreamReader) {#constructor_7}

ينشئ كائنًا جديدًا من فئة [`Project`](../) من كائن StreamReader.

```csharp
public Project(StreamReader reader)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| قارئ | StreamReader | قارئ الدفق الذي يتم منه تحميل القالب. |

## الأمثلة

يوضح كيفية قراءة ملفات MPX بترميز محدد.

```csharp
using (var streamReader = new StreamReader(DataDir + "EUC-KR-encoding.mpx", System.Text.Encoding.GetEncoding("ISO-8859-1")))
{
    var project = new Project(streamReader);
    Console.WriteLine(project.RootTask.Children.ToList()[0].Get(Tsk.Name));
    project.Save(OutDir + "WorkingWithEncodings_out.mpx", SaveFileFormat.Mpx);
}
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, PrimaveraReadOptions) {#constructor_11}

ينشئ كائنًا جديدًا من فئة [`Project`](../) من قالب (ملف MPP أو MPT موجود) باستخدام الكائن المحدد من فئة [`PrimaveraReadOptions`](../../primaverareadoptions/).

```csharp
public Project(string projectTemplate, PrimaveraReadOptions options)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| projectTemplate | سلسلة | المسار إلى القالب لإنشاء المشروع منه |
| options | PrimaveraReadOptions | الكائن المحدد من فئة [`PrimaveraReadOptions`](../../primaverareadoptions/). |

## الأمثلة

يوضح كيفية قراءة مشروع من ملف Primavera XML أو Primavera XER يحتوي على عدة مشاريع باستخدام خيارات قراءة Primavera.

```csharp
var options = new PrimaveraReadOptions()
{
    ProjectUid = 4557
};

// يعيد مشروعًا بمعرف UID خاص.
var project = new Project(DataDir + "Project.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### انظر أيضًا

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(DbSettings) {#constructor_1}

ينشئ كائنًا جديدًا من فئة [`Project`](../) لقراءة البيانات من قاعدة بيانات يتم تحديدها بواسطة كائن [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/).

```csharp
public Project(DbSettings settings)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| settings | DbSettings | الكائن المحدد من فئة [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/). |

## الأمثلة

يوضح كيفية استيراد مشروع من قاعدة بيانات Primavera باستخدام إعدادات قاعدة البيانات.

```csharp
var sb = new SqlConnectionStringBuilder
{
    DataSource = "192.168.56.3,1433",
    Encrypt = true,
    TrustServerCertificate = true,
    InitialCatalog = "PrimaveraEDB",
    NetworkLibrary = "DBMSSOCN",
    UserID = "privuser",
    Password = "***",
};

// إنشاء مثيل جديد من فئة PrimaveraDbSettings باستخدام سلسلة الاتصال ومعرف المشروع
var settings = new PrimaveraDbSettings(sb.ConnectionString, 4502);

// إنشاء كائن جديد من فئة Project
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### انظر أيضًا

* class [DbSettings](../../../aspose.tasks.connectivity/dbsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, ParseErrorCallback) {#constructor_4}

ينشئ كائنًا جديدًا من فئة [`Project`](../) من قالب (ملف mpp أو mpt موجود).

```csharp
public Project(Stream stream, ParseErrorCallback parseErrorHandler)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| دفق | دفق | دفق لتحميل القالب منه. |
| parseErrorHandler | ParseErrorCallback | طريقة الاستدعاء المحددة لمعالجة أخطاء تحليل XML. |

## الأمثلة

يظهر كيفية قراءة مشروع من ملف XML يحتوي على أحرف غير صالحة.

```csharp
public static void LoadProjectFromStream(string brokenXmlData)
{
    // افتح الدفق الذي يحتوي على XML مع فترات زمنية مكسورة
    byte[] bytes = Encoding.UTF8.GetBytes(brokenXmlData);
    using (var stream = new MemoryStream(bytes))
    {
        var project = new Project(stream, CustomDurationHandlerForStream2);
        Console.WriteLine(project.Get(Prj.Name));
    }
}

public static object CustomDurationHandlerForStream2(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Debug.Print("Object field : {0}, Invalid value : {1}", args.FieldName, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var newValue = Duration.ParseTimeSpan(duration);
    Debug.Print("New value : {0}", newValue);
    return newValue;
}
```

### انظر أيضًا

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, string) {#constructor_6}

ينشئ كائنًا جديدًا من فئة [`Project`](../) من قالب (ملف mpp أو mpt موجود).

```csharp
public Project(Stream stream, string protectionPassword)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| دفق | دفق | دفق لتحميل القالب منه. |
| protectionPassword | سلسلة | كلمة مرور الحماية. |

## ملاحظات

قراءة الملفات المحمية بكلمة مرور مدعومة حاليًا لتنسيق ملف MSP 2003 فقط.

## الأمثلة

يظهر كيفية التحقق مما إذا كان ملف MPP محميًا بكلمة مرور.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "PasswordProtected.mpp");
Console.WriteLine("Is file password protected?:" + info.IsPasswordProtected);
```

يظهر كيفية قراءة ملفات MPP المحمية بكلمة مرور من دفق.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var project = new Project(stream, "password");
    Console.WriteLine(project.Get(Prj.Name));
}
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, LoadOptions) {#constructor_9}

ينشئ مثيلًا جديدًا من الفئة [`Project`](../) من قالب (ملف mpp أو mpt موجود) باستخدام المثيل المحدد من الفئة [`LoadOptions`](../../loadoptions/).

```csharp
public Project(string projectTemplate, LoadOptions options)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| projectTemplate | سلسلة | المسار إلى القالب لإنشاء المشروع منه |
| options | LoadOptions | المثيل المحدد من الفئة [`LoadOptions`](../../loadoptions/). |

## الأمثلة

يظهر كيفية تحميل المشروع من ملف باستخدام المثيل &lt;see cref="Aspose.Tasks.LoadOptions"/&gt;.

```csharp
var options = new LoadOptions
{
    Password = "password"
};
var project = new Project(DataDir + "PasswordProtectedProject.mpp", options);
Console.WriteLine(project.Get(Prj.Name));
```

يظهر كيفية قراءة مشروع من ملف Primavera XML مع خطأ في التحليل.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};

var loadOptions = new LoadOptions()
{
    PrimaveraReadOptions = options,
    ErrorHandler = CustomDurationHandlerForFile
};

// يعيد مشروعًا بمعرف UID خاص.
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

### انظر أيضًا

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, LoadOptions) {#constructor_3}

ينشئ مثيلًا جديدًا من الفئة [`Project`](../) من الدفق باستخدام المثيل المحدد من الفئة [`LoadOptions`](../../loadoptions/).

```csharp
public Project(Stream stream, LoadOptions options)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| دفق | دفق | دفق فئة المشروع Streamclass |
| options | LoadOptions | المثيل المحدد من الفئة [`LoadOptions`](../../loadoptions/). |

## الأمثلة

يظهر كيفية تحميل المشروع من دفق باستخدام المثيل &lt;see cref="Aspose.Tasks.LoadOptions"/&gt;.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### انظر أيضًا

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


