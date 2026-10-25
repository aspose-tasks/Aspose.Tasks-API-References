---
title: "Project.Print"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Печатает проект на принтере по умолчанию с настройками принтера по умолчанию, используя стандартный контроллер печати без пользовательского интерфейса."
type: docs
weight: 1140
url: /ru/net/aspose.tasks/project/print/
---
## Print() {#print}

Печатает проект на принтере по умолчанию с настройками принтера по умолчанию, используя стандартный (без пользовательского интерфейса) контроллер печати.

```csharp
public void Print()
```

## Примеры

Показывает, как распечатать проект.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Print();
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrintOptions) {#print_1}

Печатает проект на принтере по умолчанию с настройками принтера по умолчанию и пользовательскими параметрами сохранения, используя стандартный (без пользовательского интерфейса) контроллер печати.

```csharp
public void Print(PrintOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| options | PrintOptions | указанный экземпляр класса [`PrintOptions`](../../../aspose.tasks.saving/printoptions/). |

## Примеры

Показывает, как распечатать проект, используя параметры печати.

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

### См. также

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(string) {#print_6}

Печатает проект на указанном принтере с настройками принтера по умолчанию, используя стандартный (без пользовательского интерфейса) контроллер печати.

```csharp
public void Print(string printerName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| printerName | Строка | Указанное имя принтера. |

## Примеры

Показывает, как распечатать проект на выбранном принтере.

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

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings) {#print_2}

Печатает проект в соответствии с указанными настройками принтера, используя стандартный (без пользовательского интерфейса) контроллер печати.

```csharp
public void Print(PrinterSettings printerSettings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| printerSettings | PrinterSettings | указанный экземпляр класса PrinterSettings. |

## Примеры

Показывает, как использовать настройки принтера для печати проекта.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Печать первых двух страниц
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings);
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, string) {#print_5}

Печатает проект в соответствии с указанными настройками принтера, используя стандартный (без пользовательского интерфейса) контроллер печати.

```csharp
public void Print(PrinterSettings printerSettings, string documentName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| printerSettings | PrinterSettings | указанный экземпляр класса PrinterSettings. |
| documentName | Строка | имя документа для отображения (например, в диалоговом окне статуса печати или в очереди принтера). |

## Примеры

Показывает, как использовать настройки принтера и имя документа для печати проекта.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Печать первых двух страниц
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, "Document #1");
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions) {#print_3}

Печатает проект в соответствии с указанными настройками принтера и пользовательскими параметрами сохранения, используя стандартный (без пользовательского интерфейса) контроллер печати.

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| printerSettings | PrinterSettings | указанный экземпляр класса PrinterSettings. |
| options | PrintOptions | указанный экземпляр класса [`PrintOptions`](../../../aspose.tasks.saving/printoptions/). |

## Примеры

Показывает, как использовать параметры принтера и настройки для печати проекта.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// Печать первых двух страниц
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options);
```

### См. также

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions, string) {#print_4}

Печатает проект в соответствии с указанными настройками принтера, пользовательскими параметрами сохранения и указанным именем документа, используя стандартный (без пользовательского интерфейса) контроллер печати.

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options, string documentName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| printerSettings | PrinterSettings | указанный экземпляр класса PrinterSettings. |
| options | PrintOptions | указанный экземпляр класса [`PrintOptions`](../../../aspose.tasks.saving/printoptions/). |
| documentName | Строка | имя документа для отображения (например, в диалоговом окне статуса печати или в очереди принтера). |

## Примеры

Показывает, как использовать параметры принтера, настройки принтера и имя документа для печати проекта.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// Печать первых двух страниц
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options, "My project name");
```

### См. также

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


