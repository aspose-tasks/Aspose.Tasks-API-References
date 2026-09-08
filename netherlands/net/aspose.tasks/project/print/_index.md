---
title: "Project.Print"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project-methode. Print het project naar de standaardprinter met standaardprinterinstellingen met behulp van de standaard printcontroller zonder gebruikersinterface"
type: docs
weight: 1140
url: /nl/net/aspose.tasks/project/print/
---
## Print() {#print}

Print het project naar de standaardprinter met de standaardprinterinstellingen met behulp van de standaard (geen gebruikersinterface) printcontroller.

```csharp
public void Print()
```

## Voorbeelden

Toont hoe een project af te drukken.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Print();
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrintOptions) {#print_1}

Print het project naar de standaardprinter met de standaardprinterinstellingen en aangepaste opslagopties met behulp van de standaard (geen gebruikersinterface) printcontroller.

```csharp
public void Print(PrintOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| options | PrintOptions | de opgegeven instantie van de [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) klasse. |

## Voorbeelden

Toont hoe een project af te drukken met behulp van printopties.

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

### Zie ook

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(string) {#print_6}

Print het project naar de opgegeven printer met de standaardprinterinstellingen met behulp van de standaard (geen gebruikersinterface) printcontroller.

```csharp
public void Print(string printerName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| printerName | String | Opgegeven printernaam. |

## Voorbeelden

Toont hoe het project af te drukken op de geselecteerde printer.

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

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings) {#print_2}

Print het project volgens de opgegeven printerinstellingen met behulp van de standaard (geen gebruikersinterface) printcontroller.

```csharp
public void Print(PrinterSettings printerSettings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| printerSettings | PrinterSettings | de opgegeven instantie van de PrinterSettings-klasse. |

## Voorbeelden

Toont hoe printerinstellingen te gebruiken om het project af te drukken.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Print de eerste twee pagina's
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings);
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, string) {#print_5}

Print het project volgens de opgegeven printerinstellingen met behulp van de standaard (geen gebruikersinterface) printcontroller.

```csharp
public void Print(PrinterSettings printerSettings, string documentName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| printerSettings | PrinterSettings | de opgegeven instantie van de PrinterSettings-klasse. |
| documentName | String | de documentnaam om weer te geven (bijvoorbeeld in een afdrukstatusdialoogvenster of printerwachtrij). |

## Voorbeelden

Toont hoe printerinstellingen en een documentnaam te gebruiken om het project af te drukken.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Print de eerste twee pagina's
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, "Document #1");
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions) {#print_3}

Print het project volgens de opgegeven printerinstellingen en aangepaste opslagopties met behulp van de standaard (geen gebruikersinterface) printcontroller.

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| printerSettings | PrinterSettings | de opgegeven instantie van de PrinterSettings-klasse. |
| options | PrintOptions | de opgegeven instantie van de [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) klasse. |

## Voorbeelden

Toont hoe printeropties en -instellingen te gebruiken om het project af te drukken.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// Print de eerste twee pagina's
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options);
```

### Zie ook

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions, string) {#print_4}

Print het project volgens de opgegeven printerinstellingen, aangepaste opslagopties en de opgegeven documentnaam met behulp van de standaard (geen gebruikersinterface) printcontroller.

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options, string documentName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| printerSettings | PrinterSettings | de opgegeven instantie van de PrinterSettings-klasse. |
| options | PrintOptions | de opgegeven instantie van de [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) klasse. |
| documentName | String | de documentnaam om weer te geven (bijvoorbeeld in een afdrukstatusdialoogvenster of printerwachtrij). |

## Voorbeelden

Toont hoe printeropties, printerinstellingen en documentnaam te gebruiken om het project af te drukken.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// Print de eerste twee pagina's
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options, "My project name");
```

### Zie ook

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


