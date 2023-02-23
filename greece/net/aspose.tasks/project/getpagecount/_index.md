---
title: GetPageCount
second_title: Aspose.Tasks για Αναφορά API .NET
description: Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας το δεδομένοSaveOptionsaspose.tasks.saving/saveoptions/ .
type: docs
weight: 1080
url: /el/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας το δεδομένο[`SaveOptions`](../../../aspose.tasks.saving/saveoptions/) .

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| saveOptions | SaveOptions | Οι επιλογές αποθήκευσης για την καταμέτρηση σελίδων. |

### Επιστρεφόμενη Αξία

ένα πλήθος σελίδων προς απόδοση.

### Παραδείγματα

Σε αυτό το παράδειγμα, η παρουσία του HtmlSaveOptions και ο αριθμός των σελίδων στο προκύπτον HTML εγγράφονται στην κονσόλα.

```csharp
[C#]
Project project = new Project(@"test.mpp");
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
    IncludeProjectNameInPageHeader = false,
    IncludeProjectNameInTitle = false,
    PageSize = PageSize.A4,
    Timescale = Timescale.Days,
    StartDate = project.Get(Prj.StartDate).Date,
    EndDate = project.Get(Prj.FinishDate).Date
};

Console.WriteLine(project.GetPageCount(saveOptions));
```

### Δείτε επίσης

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* χώρος ονομάτων [Aspose.Tasks](../../project/)
* συνέλευση [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας την προεπιλογή[`Timescale`](../../../aspose.tasks.visualization/timescale/) (Ημέρες).

```csharp
public int GetPageCount()
```

### Επιστρεφόμενη Αξία

Πλήθος σελίδων προς απόδοση.

### Δείτε επίσης

* class [Project](../)
* χώρος ονομάτων [Aspose.Tasks](../../project/)
* συνέλευση [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας το δεδομένο[`Timescale`](../../../aspose.tasks.visualization/timescale/) .

```csharp
public int GetPageCount(Timescale scale)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| scale | Timescale | Η κλίμακα για τη λήψη του πλήθους σελίδων. |

### Επιστρεφόμενη Αξία

Πλήθος σελίδων προς απόδοση.

### Δείτε επίσης

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* χώρος ονομάτων [Aspose.Tasks](../../project/)
* συνέλευση [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας την προεπιλογή[`Timescale`](../../../aspose.tasks.visualization/timescale/) (Ημέρες) και δίνονται[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)

```csharp
public int GetPageCount(PresentationFormat format)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| format | PresentationFormat | Η μορφή για τη λήψη του πλήθους σελίδων. |

### Επιστρεφόμενη Αξία

Πλήθος σελίδων προς απόδοση.

### Δείτε επίσης

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* χώρος ονομάτων [Aspose.Tasks](../../project/)
* συνέλευση [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας το δεδομένο[`Timescale`](../../../aspose.tasks.visualization/timescale/) και[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) .

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| format | PresentationFormat | Η μορφή για τη λήψη του πλήθους σελίδων. |
| scale | Timescale | Η κλίμακα για τη λήψη του πλήθους σελίδων. |

### Επιστρεφόμενη Αξία

ένα πλήθος σελίδων προς απόδοση.

### Δείτε επίσης

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* χώρος ονομάτων [Aspose.Tasks](../../project/)
* συνέλευση [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας το δεδομένο[`Timescale`](../../../aspose.tasks.visualization/timescale/) ,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) και εύρος ημερομηνιών.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageSize | PageSize | Το μέγεθος για να λάβετε τον αριθμό σελίδων. |
| scale | Timescale | Η κλίμακα για τη λήψη του πλήθους σελίδων. |
| startDate | DateTime | Η ημερομηνία έναρξης για τη λήψη του πλήθους σελίδων. |
| endDate | DateTime | Η ημερομηνία λήξης για να λάβετε τον αριθμό σελίδων. |

### Επιστρεφόμενη Αξία

Πλήθος σελίδων προς απόδοση.

### Δείτε επίσης

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* χώρος ονομάτων [Aspose.Tasks](../../project/)
* συνέλευση [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας το δεδομένο[`Timescale`](../../../aspose.tasks.visualization/timescale/) και[`PageSize`](../../../aspose.tasks.visualization/pagesize/) .

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageSize | PageSize | Το μέγεθος για να λάβετε τον αριθμό σελίδων. |
| scale | Timescale | Η κλίμακα για τη λήψη του πλήθους σελίδων. |

### Επιστρεφόμενη Αξία

Πλήθος σελίδων προς απόδοση.

### Δείτε επίσης

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* χώρος ονομάτων [Aspose.Tasks](../../project/)
* συνέλευση [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
