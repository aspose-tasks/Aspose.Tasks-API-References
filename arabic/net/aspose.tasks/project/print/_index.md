---
title: "Project.Print"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. تطبع المشروع إلى الطابعة الافتراضية بإعدادات الطابعة الافتراضية باستخدام وحدة تحكم الطباعة القياسية بدون واجهة مستخدم."
type: docs
weight: 1140
url: /ar/net/aspose.tasks/project/print/
---
## Print() {#print}

يطبع المشروع إلى الطابعة الافتراضية بإعدادات الطابعة الافتراضية باستخدام وحدة التحكم في الطباعة القياسية (بدون واجهة مستخدم).

```csharp
public void Print()
```

## الأمثلة

يوضح كيفية طباعة مشروع.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Print();
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrintOptions) {#print_1}

يطبع المشروع إلى الطابعة الافتراضية بإعدادات الطابعة الافتراضية وخيارات حفظ مخصصة باستخدام وحدة التحكم في الطباعة القياسية (بدون واجهة مستخدم).

```csharp
public void Print(PrintOptions options)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| options | PrintOptions | المثيل المحدد من الفئة [`PrintOptions`](../../../aspose.tasks.saving/printoptions/). |

## الأمثلة

يوضح كيفية طباعة مشروع باستخدام خيارات الطباعة.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.ThirdsOfMonths
};
if (project.GetPageCount(Timescale.ThirdsOfMonths) <= 280)
{
    project.Print(options);
}
```

### انظر أيضًا

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(string) {#print_6}

يطبع المشروع إلى الطابعة المحددة بإعدادات الطابعة الافتراضية باستخدام وحدة التحكم في الطباعة القياسية (بدون واجهة مستخدم).

```csharp
public void Print(string printerName)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| printerName | سلسلة | اسم الطابعة المحدد. |

## الأمثلة

يوضح كيفية طباعة المشروع على الطابعة المحددة.

```csharp
var project = new Project(DataDir + "Project2.mpp");

foreach (string printer in PrinterSettings.InstalledPrinters)
{
    if (!printer.ToUpperInvariant().Contains("Microsoft Print to PDF".ToUpperInvariant()))
    {
        continue;
    }

    project.Print(printer);
    break;
}
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings) {#print_2}

يطبع المشروع وفقًا لإعدادات الطابعة المحددة باستخدام وحدة التحكم في الطباعة القياسية (بدون واجهة مستخدم).

```csharp
public void Print(PrinterSettings printerSettings)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| إعدادات الطابعة | إعدادات الطابعة | المثيل المحدد من فئة PrinterSettings. |

## الأمثلة

يظهر كيفية استخدام إعدادات الطابعة لطباعة المشروع.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// طباعة الصفحتين الأوليين
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings);
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, string) {#print_5}

يطبع المشروع وفقًا لإعدادات الطابعة المحددة باستخدام وحدة التحكم في الطباعة القياسية (بدون واجهة مستخدم).

```csharp
public void Print(PrinterSettings printerSettings, string documentName)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| إعدادات الطابعة | إعدادات الطابعة | المثيل المحدد من فئة PrinterSettings. |
| اسم المستند | سلسلة | اسم المستند لعرضه (على سبيل المثال، في مربع حوار حالة الطباعة أو قائمة انتظار الطابعة). |

## الأمثلة

يظهر كيفية استخدام إعدادات الطابعة واسم المستند لطباعة المشروع.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// طباعة الصفحتين الأوليين
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, "Document #1");
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions) {#print_3}

يطبع المشروع وفقًا لإعدادات الطابعة المحددة وخيارات حفظ مخصصة باستخدام وحدة التحكم في الطباعة القياسية (بدون واجهة مستخدم).

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| إعدادات الطابعة | إعدادات الطابعة | المثيل المحدد من فئة PrinterSettings. |
| options | PrintOptions | المثيل المحدد من الفئة [`PrintOptions`](../../../aspose.tasks.saving/printoptions/). |

## الأمثلة

يظهر كيفية استخدام خيارات الطابعة والإعدادات لطباعة المشروع.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// طباعة الصفحتين الأوليين
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options);
```

### انظر أيضًا

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions, string) {#print_4}

يطبع المشروع وفقًا لإعدادات الطابعة المحددة، خيارات حفظ مخصصة واسم المستند المحدد باستخدام وحدة التحكم في الطباعة القياسية (بدون واجهة مستخدم).

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options, string documentName)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| إعدادات الطابعة | إعدادات الطابعة | المثيل المحدد من فئة PrinterSettings. |
| options | PrintOptions | المثيل المحدد من الفئة [`PrintOptions`](../../../aspose.tasks.saving/printoptions/). |
| اسم المستند | سلسلة | اسم المستند لعرضه (على سبيل المثال، في مربع حوار حالة الطباعة أو قائمة انتظار الطابعة). |

## الأمثلة

يظهر كيفية استخدام خيارات الطابعة وإعدادات الطابعة واسم المستند لطباعة المشروع.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// طباعة الصفحتين الأوليين
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options, "My project name");
```

### انظر أيضًا

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


