---
title: Project.Print
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Prints project to the default printer with default printer settings using the standard no User Interface print controller
type: docs
weight: 1130
url: /net/aspose.tasks/project/print/
---
## Print() {#print}

Prints project to the default printer with default printer settings using the standard (no User Interface) print controller.

```csharp
public void Print()
```

## Examples

Shows how to print a project.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Print();
```

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrintOptions) {#print_1}

Prints project to the default printer with default printer settings and custom save options using the standard (no User Interface) print controller.

```csharp
public void Print(PrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | PrintOptions | the specified instance of the [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) class. |

## Examples

Shows how to print a project by using of print options.

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

### See Also

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(string) {#print_6}

Prints project to the specified printer with default printer settings using the standard (no User Interface) print controller.

```csharp
public void Print(string printerName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| printerName | String | Specified printer name. |

## Examples

Shows how to print the project on the selected printer.

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

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings) {#print_2}

Prints project according to the specified printer settings using the standard (no User Interface) print controller.

```csharp
public void Print(PrinterSettings printerSettings)
```

| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | PrinterSettings | the specified instance of the PrinterSettings class. |

## Examples

Shows how to use printer settings to print the project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Print first two pages
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings);
```

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, string) {#print_5}

Prints project according to the specified printer settings using the standard (no User Interface) print controller.

```csharp
public void Print(PrinterSettings printerSettings, string documentName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | PrinterSettings | the specified instance of the PrinterSettings class. |
| documentName | String | the document name to display (for example, in a print status dialog box or printer queue). |

## Examples

Shows how to use printer settings and a document name to print the project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Print first two pages
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, "Document #1");
```

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions) {#print_3}

Prints project according to the specified printer settings and custom save options using the standard (no User Interface) print controller.

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | PrinterSettings | the specified instance of the PrinterSettings class. |
| options | PrintOptions | the specified instance of the [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) class. |

## Examples

Shows how to use printer options and settings to print the project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// Print first two pages
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options);
```

### See Also

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions, string) {#print_4}

Prints project according to the specified printer settings, custom save options and the specified document name using the standard (no User Interface) print controller.

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options, string documentName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | PrinterSettings | the specified instance of the PrinterSettings class. |
| options | PrintOptions | the specified instance of the [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) class. |
| documentName | String | the document name to display (for example, in a print status dialog box or printer queue). |

## Examples

Shows how to use printer options, printer settings and document name to print the project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// Print first two pages
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options, "My project name");
```

### See Also

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


