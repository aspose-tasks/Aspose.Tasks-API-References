---
title: "Project.GetPageCount"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Project. Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας τις δοσμένες SaveOptions"
type: docs
weight: 1110
url: /el/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας τις δοσμένες [`SaveOptions`](../../../aspose.tasks.saving/saveoptions/).

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| saveOptions | SaveOptions | Οι επιλογές αποθήκευσης για τις οποίες θα ληφθεί ο αριθμός σελίδων. |

### Τιμή Επιστροφής

ένας αριθμός σελίδων που θα αποδοθεί.

## Παραδείγματα

Σε αυτό το παράδειγμα, η παρουσία του HtmlSaveOptions και ο αριθμός των σελίδων στο παραγόμενο HTML γράφονται στην κονσόλα.

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

Δείχνει πώς να λάβετε τον αριθμό σελίδων για συγκεκριμένες επιλογές αποθήκευσης.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var options = new HtmlSaveOptions
                  {
                      IncludeProjectNameInPageHeader = false,
                      IncludeProjectNameInTitle = false,
                      PageSize = PageSize.A4,
                      Timescale = Timescale.Days,
                      StartDate = project.Get(Prj.StartDate).Date,
                      EndDate = project.Get(Prj.FinishDate).Date
                  };

Console.WriteLine(project.GetPageCount(options));
```

### Δείτε επίσης

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας την προεπιλεγμένη [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Days).

```csharp
public int GetPageCount()
```

### Τιμή Επιστροφής

Αριθμός σελίδων που θα αποδοθεί.

## Παραδείγματα

Δείχνει πώς να λάβετε τον αριθμό σελίδων για διαφορετικές κλίμακες χρόνου.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Λάβετε τον αριθμό σελίδων, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας τη δεδομένη [`Timescale`](../../../aspose.tasks.visualization/timescale/).

```csharp
public int GetPageCount(Timescale scale)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| κλίμακα | Timescale | Η κλίμακα για την οποία θα ληφθεί ο αριθμός σελίδων. |

### Τιμή Επιστροφής

Αριθμός σελίδων που θα αποδοθεί.

## Παραδείγματα

Δείχνει πώς να λάβετε τον αριθμό σελίδων για διαφορετικές κλίμακες χρόνου.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Λάβετε τον αριθμό σελίδων, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### Δείτε επίσης

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας την προεπιλεγμένη [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Days) και τη δεδομένη [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)

```csharp
public int GetPageCount(PresentationFormat format)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| μορφή | PresentationFormat | Η μορφή για την οποία θα ληφθεί ο αριθμός σελίδων. |

### Τιμή Επιστροφής

Αριθμός σελίδων που θα αποδοθεί.

## Παραδείγματα

Δείχνει πώς να λάβετε τον αριθμό σελίδων ανά μορφή παρουσίασης και κλίμακα χρόνου.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Λάβετε τον αριθμό σελίδων για Ημέρες (προεπιλογή), Μήνες και ThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### Δείτε επίσης

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας τη δεδομένη [`Timescale`](../../../aspose.tasks.visualization/timescale/) και την [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/).

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| μορφή | PresentationFormat | Η μορφή για την οποία θα ληφθεί ο αριθμός σελίδων. |
| κλίμακα | Timescale | Η κλίμακα για την οποία θα ληφθεί ο αριθμός σελίδων. |

### Τιμή Επιστροφής

ένας αριθμός σελίδων που θα αποδοθεί.

## Παραδείγματα

Δείχνει πώς να λάβετε τον αριθμό σελίδων ανά μορφή παρουσίασης και κλίμακα χρόνου.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Λάβετε τον αριθμό σελίδων για Ημέρες (προεπιλογή), Μήνες και ThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### Δείτε επίσης

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας τη δεδομένη [`Timescale`](../../../aspose.tasks.visualization/timescale/), την [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) και το εύρος ημερομηνιών.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageSize | PageSize | Το μέγεθος για το οποίο θα ληφθεί ο αριθμός σελίδων. |
| κλίμακα | Timescale | Η κλίμακα για την οποία θα ληφθεί ο αριθμός σελίδων. |
| startDate | DateTime | Η ημερομηνία έναρξης για την οποία θα ληφθεί ο αριθμός σελίδων. |
| endDate | DateTime | Η ημερομηνία λήξης για την οποία θα ληφθεί ο αριθμός σελίδων. |

### Τιμή Επιστροφής

Αριθμός σελίδων που θα αποδοθεί.

## Παραδείγματα

Δείχνει πώς να λάβετε τον αριθμό σελίδων ανά μέγεθος σελίδας, κλίμακα χρόνου, ημερομηνίες έναρξης και λήξης.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(
    PageSize.A3,
    Timescale.Months,
    project.Get(Prj.StartDate) - TimeSpan.FromDays(10),
    project.Get(Prj.FinishDate) + TimeSpan.FromDays(30));

Console.WriteLine(pageCount);
```

### Δείτε επίσης

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας τη δεδομένη [`Timescale`](../../../aspose.tasks.visualization/timescale/) και την [`PageSize`](../../../aspose.tasks.visualization/pagesize/).

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageSize | PageSize | Το μέγεθος για το οποίο θα ληφθεί ο αριθμός σελίδων. |
| κλίμακα | Timescale | Η κλίμακα για την οποία θα ληφθεί ο αριθμός σελίδων. |

### Τιμή Επιστροφής

Αριθμός σελίδων που θα αποδοθεί.

## Παραδείγματα

Δείχνει πώς να υπολογίσετε τον αριθμό των σελίδων βάσει μεγέθους σελίδας και χρονολογικής κλίμακας.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(PageSize.A3, Timescale.Months);

Console.WriteLine(pageCount);
```

### Δείτε επίσης

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


