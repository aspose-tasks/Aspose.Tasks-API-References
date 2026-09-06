---
title: "Project.Print"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 方法。使用标准的无用户界面打印控制器，使用默认打印机设置将项目打印到默认打印机"
type: docs
weight: 1140
url: /zh/net/aspose.tasks/project/print/
---
## Print() {#print}

使用标准（无用户界面）打印控制器，将项目打印到默认打印机，使用默认打印机设置。

```csharp
public void Print()
```

## 示例

展示如何打印项目。

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Print();
```

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrintOptions) {#print_1}

使用标准（无用户界面）打印控制器，将项目打印到默认打印机，使用默认打印机设置和自定义保存选项。

```csharp
public void Print(PrintOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | PrintOptions | 指定的 [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) 类的实例。 |

## 示例

展示如何通过使用打印选项来打印项目。

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

### 另见

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(string) {#print_6}

使用标准（无用户界面）打印控制器，将项目打印到指定打印机，使用默认打印机设置。

```csharp
public void Print(string printerName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| printerName | 字符串 | 指定的打印机名称。 |

## 示例

展示如何在选定的打印机上打印项目。

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

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings) {#print_2}

使用标准（无用户界面）打印控制器，根据指定的打印机设置打印项目。

```csharp
public void Print(PrinterSettings printerSettings)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| printerSettings | PrinterSettings | 指定的 PrinterSettings 类实例。 |

## 示例

展示如何使用打印机设置来打印项目。

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 打印前两页
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings);
```

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, string) {#print_5}

使用标准（无用户界面）打印控制器，根据指定的打印机设置打印项目。

```csharp
public void Print(PrinterSettings printerSettings, string documentName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| printerSettings | PrinterSettings | 指定的 PrinterSettings 类实例。 |
| documentName | 字符串 | 要显示的文档名称（例如，在打印状态对话框或打印机队列中）。 |

## 示例

展示如何使用打印机设置和文档名称来打印项目。

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 打印前两页
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, "Document #1");
```

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions) {#print_3}

使用标准（无用户界面）打印控制器，根据指定的打印机设置和自定义保存选项打印项目。

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| printerSettings | PrinterSettings | 指定的 PrinterSettings 类实例。 |
| options | PrintOptions | 指定的 [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) 类的实例。 |

## 示例

展示如何使用打印机选项和设置来打印项目。

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// 打印前两页
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options);
```

### 另见

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions, string) {#print_4}

使用标准（无用户界面）打印控制器，根据指定的打印机设置、自定义保存选项和指定的文档名称打印项目。

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options, string documentName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| printerSettings | PrinterSettings | 指定的 PrinterSettings 类实例。 |
| options | PrintOptions | 指定的 [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) 类的实例。 |
| documentName | 字符串 | 要显示的文档名称（例如，在打印状态对话框或打印机队列中）。 |

## 示例

展示如何使用打印机选项、打印机设置和文档名称来打印项目。

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// 打印前两页
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options, "My project name");
```

### 另见

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


