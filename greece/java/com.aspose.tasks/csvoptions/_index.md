---
title: "CsvOptions"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση του έργου σε CSV."
type: docs
weight: 56
url: /el/java/com.aspose.tasks/csvoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class CsvOptions extends SimpleSaveOptions
```

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση του έργου σε CSV.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [CsvOptions()](#CsvOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [CsvOptions](../../com.aspose/tasks/csvoptions) που μπορεί να χρησιμοποιηθεί για την αποθήκευση του έργου σε μορφή CSV. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getDataCategory()](#getDataCategory--) | Λαμβάνει μια κατηγορία δεδομένων για αποθήκευση. |
| [getEncoding()](#getEncoding--) | Λαμβάνει μια κωδικοποίηση για αποθήκευση CSV. |
| [getIncludeHeaders()](#getIncludeHeaders--) | Λαμβάνει μια τιμή που υποδεικνύει αν θα συμπεριληφθούν κεφαλίδες ή όχι (η προεπιλεγμένη τιμή είναι TRUE). |
| [getTextDelimiter()](#getTextDelimiter--) | Λαμβάνει έναν διαχωριστή κειμένου. |
| [getView()](#getView--) | Λαμβάνει μια λίστα των στηλών προβολής ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) για αποθήκευση σε μορφή XLSX. |
| [setDataCategory(int value)](#setDataCategory-int-) | Ορίζει μια κατηγορία δεδομένων για αποθήκευση. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Ορίζει μια κωδικοποίηση για αποθήκευση CSV. |
| [setIncludeHeaders(boolean value)](#setIncludeHeaders-boolean-) | Ορίζει μια τιμή που υποδεικνύει αν θα συμπεριληφθούν κεφαλίδες ή όχι (η προεπιλεγμένη τιμή είναι TRUE). |
| [setTextDelimiter(int value)](#setTextDelimiter-int-) | Ορίζει έναν διαχωριστή κειμένου. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Ορίζει μια λίστα των στηλών προβολής ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) για αποθήκευση σε μορφή XLSX. |
### CsvOptions() {#CsvOptions--}
```
public CsvOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [CsvOptions](../../com.aspose/tasks/csvoptions) που μπορεί να χρησιμοποιηθεί για την αποθήκευση του έργου σε μορφή CSV.

### getDataCategory() {#getDataCategory--}
```
public final int getDataCategory()
```


Λαμβάνει μια κατηγορία δεδομένων για αποθήκευση.

**Returns:**
int - μια κατηγορία δεδομένων για αποθήκευση.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Λαμβάνει μια κωδικοποίηση για αποθήκευση CSV.

**Returns:**
java.nio.charset.Charset - μια κωδικοποίηση για αποθήκευση CSV.
### getIncludeHeaders() {#getIncludeHeaders--}
```
public final boolean getIncludeHeaders()
```


Λαμβάνει μια τιμή που υποδεικνύει αν θα συμπεριληφθούν κεφαλίδες ή όχι (η προεπιλεγμένη τιμή είναι TRUE).

**Returns:**
boolean - μια τιμή που υποδεικνύει αν θα συμπεριληφθούν κεφαλίδες ή όχι (η προεπιλεγμένη τιμή είναι TRUE).
### getTextDelimiter() {#getTextDelimiter--}
```
public final int getTextDelimiter()
```


Λαμβάνει έναν διαχωριστή κειμένου.

**Returns:**
int - ένας διαχωριστής κειμένου.
### getView() {#getView--}
```
public final ProjectView getView()
```


Λαμβάνει μια λίστα των στηλών προβολής ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) για αποθήκευση σε μορφή XLSX. Εάν δεν οριστεί, τότε αποθηκεύονται οι προεπιλεγμένες στήλες.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setDataCategory(int value) {#setDataCategory-int-}
```
public final void setDataCategory(int value)
```


Ορίζει μια κατηγορία δεδομένων για αποθήκευση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια κατηγορία δεδομένων για αποθήκευση. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Ορίζει μια κωδικοποίηση για αποθήκευση CSV.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.nio.charset.Charset | μια κωδικοποίηση για αποθήκευση CSV. |

### setIncludeHeaders(boolean value) {#setIncludeHeaders-boolean-}
```
public final void setIncludeHeaders(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει αν θα συμπεριληφθούν κεφαλίδες ή όχι (η προεπιλεγμένη τιμή είναι TRUE).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν θα συμπεριληφθούν κεφαλίδες ή όχι (η προεπιλεγμένη τιμή είναι TRUE). |

### setTextDelimiter(int value) {#setTextDelimiter-int-}
```
public final void setTextDelimiter(int value)
```


Ορίζει έναν διαχωριστή κειμένου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένας διαχωριστής κειμένου. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Ορίζει μια λίστα των στηλών προβολής ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) για αποθήκευση σε μορφή XLSX. Εάν δεν οριστεί, τότε αποθηκεύονται οι προεπιλεγμένες στήλες.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | μια λίστα των στηλών προβολής ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) για αποθήκευση σε μορφή XLSX. |

