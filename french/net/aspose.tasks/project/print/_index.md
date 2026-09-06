---
title: "Project.Print"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Project. Imprime le projet sur l’imprimante par défaut avec les paramètres d’imprimante par défaut en utilisant le contrôleur d’impression standard sans interface utilisateur"
type: docs
weight: 1140
url: /fr/net/aspose.tasks/project/print/
---
## Print() {#print}

Imprime le projet sur l’imprimante par défaut avec les paramètres d’imprimante par défaut en utilisant le contrôleur d’impression standard (sans interface utilisateur).

```csharp
public void Print()
```

## Exemples

Montre comment imprimer un projet.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Print();
```

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrintOptions) {#print_1}

Imprime le projet sur l’imprimante par défaut avec les paramètres d’imprimante par défaut et des options d’enregistrement personnalisées en utilisant le contrôleur d’impression standard (sans interface utilisateur).

```csharp
public void Print(PrintOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | PrintOptions | l’instance spécifiée de la classe [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) . |

## Exemples

Montre comment imprimer un projet en utilisant les options d’impression.

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

### Voir aussi

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(string) {#print_6}

Imprime le projet sur l’imprimante spécifiée avec les paramètres d’imprimante par défaut en utilisant le contrôleur d’impression standard (sans interface utilisateur).

```csharp
public void Print(string printerName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| printerName | Chaîne | Nom d’imprimante spécifié. |

## Exemples

Montre comment imprimer le projet sur l’imprimante sélectionnée.

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

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings) {#print_2}

Imprime le projet selon les paramètres d’imprimante spécifiés en utilisant le contrôleur d’impression standard (sans interface utilisateur).

```csharp
public void Print(PrinterSettings printerSettings)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| printerSettings | PrinterSettings | l'instance spécifiée de la classe PrinterSettings. |

## Exemples

Montre comment utiliser les paramètres d'imprimante pour imprimer le projet.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Imprimer les deux premières pages
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings);
```

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, string) {#print_5}

Imprime le projet selon les paramètres d’imprimante spécifiés en utilisant le contrôleur d’impression standard (sans interface utilisateur).

```csharp
public void Print(PrinterSettings printerSettings, string documentName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| printerSettings | PrinterSettings | l'instance spécifiée de la classe PrinterSettings. |
| documentName | Chaîne | le nom du document à afficher (par exemple, dans une boîte de dialogue d'état d'impression ou dans la file d'attente de l'imprimante). |

## Exemples

Montre comment utiliser les paramètres d'imprimante et le nom du document pour imprimer le projet.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Imprimer les deux premières pages
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, "Document #1");
```

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions) {#print_3}

Imprime le projet selon les paramètres d’imprimante spécifiés et des options d’enregistrement personnalisées en utilisant le contrôleur d’impression standard (sans interface utilisateur).

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| printerSettings | PrinterSettings | l'instance spécifiée de la classe PrinterSettings. |
| options | PrintOptions | l’instance spécifiée de la classe [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) . |

## Exemples

Montre comment utiliser les options et paramètres d'imprimante pour imprimer le projet.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// Imprimer les deux premières pages
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options);
```

### Voir aussi

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions, string) {#print_4}

Imprime le projet selon les paramètres d’imprimante spécifiés, des options d’enregistrement personnalisées et le nom de document spécifié en utilisant le contrôleur d’impression standard (sans interface utilisateur).

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options, string documentName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| printerSettings | PrinterSettings | l'instance spécifiée de la classe PrinterSettings. |
| options | PrintOptions | l’instance spécifiée de la classe [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) . |
| documentName | Chaîne | le nom du document à afficher (par exemple, dans une boîte de dialogue d'état d'impression ou dans la file d'attente de l'imprimante). |

## Exemples

Montre comment utiliser les options d'imprimante, les paramètres d'imprimante et le nom du document pour imprimer le projet.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// Imprimer les deux premières pages
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options, "My project name");
```

### Voir aussi

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


