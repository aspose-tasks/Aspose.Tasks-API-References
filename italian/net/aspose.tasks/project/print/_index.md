---
title: "Project.Print"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Project. Stampa il progetto sulla stampante predefinita con le impostazioni predefinite della stampante utilizzando il controller di stampa standard senza interfaccia utente"
type: docs
weight: 1140
url: /it/net/aspose.tasks/project/print/
---
## Print() {#print}

Stampa il progetto sulla stampante predefinita con le impostazioni predefinite della stampante usando il controller di stampa standard (senza interfaccia utente).

```csharp
public void Print()
```

## Esempi

Mostra come stampare un progetto.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Print();
```

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrintOptions) {#print_1}

Stampa il progetto sulla stampante predefinita con le impostazioni predefinite della stampante e opzioni di salvataggio personalizzate usando il controller di stampa standard (senza interfaccia utente).

```csharp
public void Print(PrintOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | PrintOptions | l'istanza specificata della classe [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) . |

## Esempi

Mostra come stampare un progetto utilizzando le opzioni di stampa.

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

### Vedi anche

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(string) {#print_6}

Stampa il progetto sulla stampante specificata con le impostazioni predefinite della stampante usando il controller di stampa standard (senza interfaccia utente).

```csharp
public void Print(string printerName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nomeStampante | Stringa | Nome stampante specificato. |

## Esempi

Mostra come stampare il progetto sulla stampante selezionata.

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

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings) {#print_2}

Stampa il progetto secondo le impostazioni della stampante specificate usando il controller di stampa standard (senza interfaccia utente).

```csharp
public void Print(PrinterSettings printerSettings)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| printerSettings | PrinterSettings | l'istanza specificata della classe PrinterSettings. |

## Esempi

Mostra come utilizzare le impostazioni della stampante per stampare il progetto.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Stampa le prime due pagine
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings);
```

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, string) {#print_5}

Stampa il progetto secondo le impostazioni della stampante specificate usando il controller di stampa standard (senza interfaccia utente).

```csharp
public void Print(PrinterSettings printerSettings, string documentName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| printerSettings | PrinterSettings | l'istanza specificata della classe PrinterSettings. |
| documentName | Stringa | il nome del documento da visualizzare (ad esempio, in una finestra di dialogo di stato di stampa o nella coda della stampante). |

## Esempi

Mostra come utilizzare le impostazioni della stampante e il nome del documento per stampare il progetto.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Stampa le prime due pagine
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, "Document #1");
```

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions) {#print_3}

Stampa il progetto secondo le impostazioni della stampante specificate e opzioni di salvataggio personalizzate usando il controller di stampa standard (senza interfaccia utente).

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| printerSettings | PrinterSettings | l'istanza specificata della classe PrinterSettings. |
| options | PrintOptions | l'istanza specificata della classe [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) . |

## Esempi

Mostra come utilizzare le opzioni e le impostazioni della stampante per stampare il progetto.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// Stampa le prime due pagine
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options);
```

### Vedi anche

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions, string) {#print_4}

Stampa il progetto secondo le impostazioni della stampante specificate, opzioni di salvataggio personalizzate e il nome del documento specificato usando il controller di stampa standard (senza interfaccia utente).

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options, string documentName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| printerSettings | PrinterSettings | l'istanza specificata della classe PrinterSettings. |
| options | PrintOptions | l'istanza specificata della classe [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) . |
| documentName | Stringa | il nome del documento da visualizzare (ad esempio, in una finestra di dialogo di stato di stampa o nella coda della stampante). |

## Esempi

Mostra come utilizzare le opzioni della stampante, le impostazioni della stampante e il nome del documento per stampare il progetto.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// Stampa le prime due pagine
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options, "My project name");
```

### Vedi anche

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


