---
title: "Project.Print"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Project. Imprime el proyecto en la impresora predeterminada con la configuración de impresora predeterminada usando el controlador de impresión estándar sin interfaz de usuario"
type: docs
weight: 1140
url: /es/net/aspose.tasks/project/print/
---
## Print() {#print}

Imprime el proyecto en la impresora predeterminada con la configuración de impresora predeterminada usando el controlador de impresión estándar (sin interfaz de usuario).

```csharp
public void Print()
```

## Ejemplos

Muestra cómo imprimir un proyecto.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Print();
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrintOptions) {#print_1}

Imprime el proyecto en la impresora predeterminada con la configuración de impresora predeterminada y opciones de guardado personalizadas usando el controlador de impresión estándar (sin interfaz de usuario).

```csharp
public void Print(PrintOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| options | PrintOptions | la instancia especificada de la clase [`PrintOptions`](../../../aspose.tasks.saving/printoptions/). |

## Ejemplos

Muestra cómo imprimir un proyecto usando opciones de impresión.

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

### Ver también

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(string) {#print_6}

Imprime el proyecto en la impresora especificada con la configuración de impresora predeterminada usando el controlador de impresión estándar (sin interfaz de usuario).

```csharp
public void Print(string printerName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerName | Cadena | Nombre de impresora especificado. |

## Ejemplos

Muestra cómo imprimir el proyecto en la impresora seleccionada.

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

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings) {#print_2}

Imprime el proyecto según la configuración de impresora especificada usando el controlador de impresión estándar (sin interfaz de usuario).

```csharp
public void Print(PrinterSettings printerSettings)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerSettings | PrinterSettings | la instancia especificada de la clase PrinterSettings. |

## Ejemplos

Muestra cómo usar la configuración de la impresora para imprimir el proyecto.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Imprimir las dos primeras páginas
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings);
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, string) {#print_5}

Imprime el proyecto según la configuración de impresora especificada usando el controlador de impresión estándar (sin interfaz de usuario).

```csharp
public void Print(PrinterSettings printerSettings, string documentName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerSettings | PrinterSettings | la instancia especificada de la clase PrinterSettings. |
| documentName | Cadena | el nombre del documento a mostrar (por ejemplo, en un cuadro de diálogo de estado de impresión o en la cola de la impresora). |

## Ejemplos

Muestra cómo usar la configuración de la impresora y un nombre de documento para imprimir el proyecto.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Imprimir las dos primeras páginas
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, "Document #1");
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions) {#print_3}

Imprime el proyecto según la configuración de impresora especificada y opciones de guardado personalizadas usando el controlador de impresión estándar (sin interfaz de usuario).

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerSettings | PrinterSettings | la instancia especificada de la clase PrinterSettings. |
| options | PrintOptions | la instancia especificada de la clase [`PrintOptions`](../../../aspose.tasks.saving/printoptions/). |

## Ejemplos

Muestra cómo usar las opciones y la configuración de la impresora para imprimir el proyecto.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// Imprimir las dos primeras páginas
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options);
```

### Ver también

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions, string) {#print_4}

Imprime el proyecto según la configuración de impresora especificada, opciones de guardado personalizadas y el nombre de documento especificado usando el controlador de impresión estándar (sin interfaz de usuario).

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options, string documentName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerSettings | PrinterSettings | la instancia especificada de la clase PrinterSettings. |
| options | PrintOptions | la instancia especificada de la clase [`PrintOptions`](../../../aspose.tasks.saving/printoptions/). |
| documentName | Cadena | el nombre del documento a mostrar (por ejemplo, en un cuadro de diálogo de estado de impresión o en la cola de la impresora). |

## Ejemplos

Muestra cómo usar las opciones de la impresora, la configuración de la impresora y el nombre del documento para imprimir el proyecto.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// Imprimir las dos primeras páginas
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options, "My project name");
```

### Ver también

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


