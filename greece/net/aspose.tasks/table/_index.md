---
title: "Κλάση Table"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Table class. Αντιπροσωπεύει έναν πίνακα στο Project."
type: docs
weight: 2320
url: /el/net/aspose.tasks/table/
---
## Table class

Αντιπροσωπεύει έναν πίνακα στο Project

```csharp
public class Table
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Table](table/)() | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `Table`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [AdjustHeaderRowHeight](../../aspose.tasks/table/adjustheaderrowheight/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το ύψος της γραμμής κεφαλίδας του πίνακα μπορεί να προσαρμοστεί. |
| [DateFormat](../../aspose.tasks/table/dateformat/) { get; set; } | Λαμβάνει ή ορίζει τη μορφή ημερομηνίας του πίνακα. |
| [LockFirstColumn](../../aspose.tasks/table/lockfirstcolumn/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η πρώτη στήλη ενός πίνακα είναι κλειδωμένη ή επεξεργάσιμη. |
| [Name](../../aspose.tasks/table/name/) { get; set; } | Λαμβάνει ή ορίζει το όνομα ενός αντικειμένου Table. |
| [RowHeight](../../aspose.tasks/table/rowheight/) { get; set; } | Λαμβάνει ή ορίζει το ύψος της γραμμής σε έναν πίνακα, όπου το ύψος της γραμμής είναι ο αριθμός των γραμμών κειμένου. |
| [ShowAddNewColumn](../../aspose.tasks/table/showaddnewcolumn/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εμφανιστεί η διεπαφή 'Add New Column'. Υποστηρίζεται από την έκδοση MSP 2010 και μεταγενέστερες. |
| [ShowInMenu](../../aspose.tasks/table/showinmenu/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το έργο εμφανίζει το όνομα του πίνακα στη λίστα αναπτυσσόμενων πινάκων στην καρτέλα Προβολή της κορδέλας. |
| [TableFields](../../aspose.tasks/table/tablefields/) { get; } | Λαμβάνει μια συλλογή TableFields που αντιπροσωπεύει τα πεδία στον πίνακα. |
| [TableType](../../aspose.tasks/table/tabletype/) { get; set; } | Λαμβάνει ή ορίζει τον τύπο πίνακα για τον καθορισμένο πίνακα. |
| [Uid](../../aspose.tasks/table/uid/) { get; } | Λαμβάνει το μοναδικό αναγνωριστικό ενός πίνακα. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [Equals](../../aspose.tasks/table/equals/)(object) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| override [GetHashCode](../../aspose.tasks/table/gethashcode/)() | Επιστρέφει έναν κωδικό κατακερματισμού για αυτόν τον Πίνακα. |

## Παραδείγματα

Δείχνει πώς να ορίσετε έναν νέο πίνακα (χρησιμοποιώντας για προβολές).

```csharp
var project = new Project(DataDir + "Project1.mpp");

// λάβετε έναν πίνακα για επεξεργασία
var table = project.Tables.ToList()[0];
Console.WriteLine("Uid of the table: " + table.Uid);
Console.WriteLine("Name of the table: " + table.Name);
Console.WriteLine("Type of the table: " + table.TableType);

// ρυθμίστε κάποιες ιδιότητες
// ορίστε μια τιμή που υποδεικνύει αν το ύψος της γραμμής κεφαλίδας του πίνακα μπορεί να προσαρμοστεί
table.AdjustHeaderRowHeight = true;

// ορίστε τη μορφή ημερομηνίας του πίνακα.
table.DateFormat = DateFormat.DateDdMmYyyy;

// ορίστε μια τιμή που υποδεικνύει αν η πρώτη στήλη ενός πίνακα είναι κλειδωμένη ή επεξεργάσιμη
table.LockFirstColumn = true;

// ορίστε το ύψος της γραμμής σε έναν πίνακα, όπου το ύψος της γραμμής είναι ο αριθμός των γραμμών κειμένου
table.RowHeight = 10;

// ορίζει μια τιμή που υποδεικνύει αν θα εμφανιστεί η διεπαφή 'Προσθήκη Νέας Στήλης'
table.ShowAddNewColumn = true;

// ορίστε μια τιμή που υποδεικνύει αν το έργο εμφανίζει το όνομα του πίνακα στη λίστα επιλογής Πίνακες στην καρτέλα Προβολή της κορδέλας
table.ShowInMenu = true;

// επιτρέπει την αποθήκευση του ενημερωμένου πίνακα
project.Save(OutDir + "WorkWithTable_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


