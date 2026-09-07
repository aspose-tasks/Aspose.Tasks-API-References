---
title: "Project.Print"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Project μέθοδος. Εκτυπώνει το project στον προεπιλεγμένο εκτυπωτή με τις προεπιλεγμένες ρυθμίσεις εκτυπωτή χρησιμοποιώντας τον τυπικό εκτυπωτή χωρίς διεπαφή χρήστη"
type: docs
weight: 1140
url: /el/net/aspose.tasks/project/print/
---
## Print() {#print}

Εκτυπώνει το έργο στον προεπιλεγμένο εκτυπωτή με τις προεπιλεγμένες ρυθμίσεις εκτυπωτή χρησιμοποιώντας τον τυπικό (χωρίς διεπαφή χρήστη) ελεγκτή εκτύπωσης.

```csharp
public void Print()
```

## Παραδείγματα

Δείχνει πώς να εκτυπώσετε ένα project.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Print();
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrintOptions) {#print_1}

Εκτυπώνει το έργο στον προεπιλεγμένο εκτυπωτή με τις προεπιλεγμένες ρυθμίσεις εκτυπωτή και προσαρμοσμένες επιλογές αποθήκευσης χρησιμοποιώντας τον τυπικό (χωρίς διεπαφή χρήστη) ελεγκτή εκτύπωσης.

```csharp
public void Print(PrintOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| options | PrintOptions | η καθορισμένη παρουσία της κλάσης [`PrintOptions`](../../../aspose.tasks.saving/printoptions/). |

## Παραδείγματα

Δείχνει πώς να εκτυπώσετε ένα project χρησιμοποιώντας τις επιλογές εκτύπωσης.

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

### Δείτε επίσης

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(string) {#print_6}

Εκτυπώνει το έργο στον καθορισμένο εκτυπωτή με τις προεπιλεγμένες ρυθμίσεις εκτυπωτή χρησιμοποιώντας τον τυπικό (χωρίς διεπαφή χρήστη) ελεγκτή εκτύπωσης.

```csharp
public void Print(string printerName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| printerName | String | Καθορισμένο όνομα εκτυπωτή. |

## Παραδείγματα

Δείχνει πώς να εκτυπώσετε το project στον επιλεγμένο εκτυπωτή.

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

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings) {#print_2}

Εκτυπώνει το έργο σύμφωνα με τις καθορισμένες ρυθμίσεις εκτυπωτή χρησιμοποιώντας τον τυπικό (χωρίς διεπαφή χρήστη) ελεγκτή εκτύπωσης.

```csharp
public void Print(PrinterSettings printerSettings)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| printerSettings | PrinterSettings | η καθορισμένη παρουσία της κλάσης PrinterSettings. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τις ρυθμίσεις εκτυπωτή για να εκτυπώσετε το έργο.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Εκτυπώστε τις πρώτες δύο σελίδες
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings);
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, string) {#print_5}

Εκτυπώνει το έργο σύμφωνα με τις καθορισμένες ρυθμίσεις εκτυπωτή χρησιμοποιώντας τον τυπικό (χωρίς διεπαφή χρήστη) ελεγκτή εκτύπωσης.

```csharp
public void Print(PrinterSettings printerSettings, string documentName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| printerSettings | PrinterSettings | η καθορισμένη παρουσία της κλάσης PrinterSettings. |
| documentName | String | το όνομα του εγγράφου για εμφάνιση (για παράδειγμα, σε παράθυρο διαλόγου κατάστασης εκτύπωσης ή στην ουρά εκτυπωτή). |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τις ρυθμίσεις εκτυπωτή και ένα όνομα εγγράφου για να εκτυπώσετε το έργο.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Εκτυπώστε τις πρώτες δύο σελίδες
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, "Document #1");
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions) {#print_3}

Εκτυπώνει το έργο σύμφωνα με τις καθορισμένες ρυθμίσεις εκτυπωτή και τις προσαρμοσμένες επιλογές αποθήκευσης χρησιμοποιώντας τον τυπικό (χωρίς διεπαφή χρήστη) ελεγκτή εκτύπωσης.

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| printerSettings | PrinterSettings | η καθορισμένη παρουσία της κλάσης PrinterSettings. |
| options | PrintOptions | η καθορισμένη παρουσία της κλάσης [`PrintOptions`](../../../aspose.tasks.saving/printoptions/). |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε επιλογές και ρυθμίσεις εκτυπωτή για να εκτυπώσετε το έργο.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// Εκτυπώστε τις πρώτες δύο σελίδες
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options);
```

### Δείτε επίσης

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions, string) {#print_4}

Εκτυπώνει το έργο σύμφωνα με τις καθορισμένες ρυθμίσεις εκτυπωτή, τις προσαρμοσμένες επιλογές αποθήκευσης και το καθορισμένο όνομα εγγράφου χρησιμοποιώντας τον τυπικό (χωρίς διεπαφή χρήστη) ελεγκτή εκτύπωσης.

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options, string documentName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| printerSettings | PrinterSettings | η καθορισμένη παρουσία της κλάσης PrinterSettings. |
| options | PrintOptions | η καθορισμένη παρουσία της κλάσης [`PrintOptions`](../../../aspose.tasks.saving/printoptions/). |
| documentName | String | το όνομα του εγγράφου για εμφάνιση (για παράδειγμα, σε παράθυρο διαλόγου κατάστασης εκτύπωσης ή στην ουρά εκτυπωτή). |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε επιλογές εκτυπωτή, ρυθμίσεις εκτυπωτή και όνομα εγγράφου για να εκτυπώσετε το έργο.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// Εκτυπώστε τις πρώτες δύο σελίδες
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options, "My project name");
```

### Δείτε επίσης

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


