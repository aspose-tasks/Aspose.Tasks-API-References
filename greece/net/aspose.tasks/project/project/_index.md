---
title: "Project.Project"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής Project. Αρχικοποιεί μια νέα παρουσία της κλάσης Project."
type: docs
weight: 10
url: /el/net/aspose.tasks/project/project/
---
## Project() {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Project`](../).

```csharp
public Project()
```

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε ένα έργο και να το αποθηκεύσετε σε μορφή MPP χωρίς να περάσετε αρχείο προτύπου MPP.

```csharp
var project = new Project();

// Το έργο θα αποθηκευτεί σε MPP χρησιμοποιώντας το εσωτερικό πρότυπο MPP.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, string) {#constructor_12}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Project`](../) από πρότυπο προστατευμένο με κωδικό (υπάρχον αρχείο mpp ή mpt).

```csharp
public Project(string projectTemplate, string protectionPassword)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| projectTemplate | String | Διαδρομή προς το πρότυπο για δημιουργία έργου. |
| protectionPassword | String | Κωδικός προστασίας. |

## Παρατηρήσεις

Η ανάγνωση αρχείων προστατευμένων με κωδικό υποστηρίζεται επί του παρόντος μόνο για τη μορφή αρχείου MSP 2003.

## Παραδείγματα

Δείχνει πώς να διαβάσετε αρχεία MPP προστατευμένα με κωδικό.

```csharp
var project = new Project(DataDir + "PasswordProtectedProject.mpp", "password");
Console.WriteLine(project.Get(Prj.Name));
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string) {#constructor_8}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Project`](../) από πρότυπο (υπάρχον αρχείο mpp ή mpt).

```csharp
public Project(string projectTemplate)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| projectTemplate | String | Διαδρομή προς το πρότυπο για δημιουργία έργου. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε ένα αρχείο MPP.

```csharp
var project = new Project(DataDir + "ReadProjectFiles.mpp");
project.Save(OutDir + "ReadProjectFiles_out.mpp", SaveFileFormat.Xml);
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, PrimaveraReadOptions) {#constructor_5}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Project`](../) από το Stream με την καθορισμένη παρουσία της κλάσης [`PrimaveraReadOptions`](../../primaverareadoptions/).

```csharp
public Project(Stream stream, PrimaveraReadOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | Ροή | Ροή του Project Streamclass |
| options | PrimaveraReadOptions | η καθορισμένη παρουσία της [`PrimaveraReadOptions`](../../primaverareadoptions/) κλάσης που επιτρέπει την προσαρμογή της ανάγνωσης των μορφών Primavera (XER ή XML). |

## Παραδείγματα

Δείχνει πώς να διαβάσετε ένα έργο από μια ροή με αρχείο Primavera XML ή Primavera XER που περιέχει πολλαπλά έργα.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open, FileAccess.Read))
{
    // Επιστρέφει έργο με ειδικό UID
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Δείτε επίσης

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, ParseErrorCallback) {#constructor_10}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Project`](../) από πρότυπο (υπάρχον αρχείο mpp ή mpt).

```csharp
public Project(string projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| projectTemplate | String | Διαδρομή προς το πρότυπο για δημιουργία έργου. |
| parseErrorHandler | ParseErrorCallback | η καθορισμένη μέθοδος callback για το χειρισμό σφαλμάτων ανάλυσης xml. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε ένα έργο από ροή με αρχείο XML με μη έγκυρους χαρακτήρες.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // ανοίξτε το αρχείο που περιέχει XML με κατεστραμμένα χρονικά διαστήματα
    var project = new Project(pathToModifiedXml, CustomDurationHandlerForFile2);
    Console.WriteLine(project.Get(Prj.Name));
}

public static object CustomDurationHandlerForFile2(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Console.WriteLine("Object field: {0}, Object field type: {1}, Invalid value: {2}", args.FieldName, args.FieldType, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var newValue = Duration.ParseTimeSpan(duration);
    Console.WriteLine("New value : {0}", newValue);
    return newValue;
}
```

### Δείτε επίσης

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της [`Project`](../) κλάσης από μια ροή.

```csharp
public Project(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | Ροή | Ροή από την οποία θα φορτωθεί ένα πρότυπο. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε αρχείο έργου XML από μια ροή.

```csharp
using (Stream stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var project = new Project(stream);
    project.Save(OutDir + "ReadProjectFileFromStream_out.xml", SaveFileFormat.Xml);
}
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(StreamReader) {#constructor_7}

Αρχικοποιεί μια νέα παρουσία της [`Project`](../) κλάσης από μια παρουσία StreamReader.

```csharp
public Project(StreamReader reader)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| αναγνώστης | StreamReader | Ο αναγνώστης ροής από τον οποίο θα φορτωθεί ένα πρότυπο. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε αρχεία MPX με συγκεκριμένη κωδικοποίηση.

```csharp
using (var streamReader = new StreamReader(DataDir + "EUC-KR-encoding.mpx", System.Text.Encoding.GetEncoding("ISO-8859-1")))
{
    var project = new Project(streamReader);
    Console.WriteLine(project.RootTask.Children.ToList()[0].Get(Tsk.Name));
    project.Save(OutDir + "WorkingWithEncodings_out.mpx", SaveFileFormat.Mpx);
}
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, PrimaveraReadOptions) {#constructor_11}

Αρχικοποιεί μια νέα παρουσία της [`Project`](../) κλάσης από ένα πρότυπο (υπάρχον αρχείο MPP ή MPT) με την καθορισμένη παρουσία της [`PrimaveraReadOptions`](../../primaverareadoptions/) κλάσης.

```csharp
public Project(string projectTemplate, PrimaveraReadOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| projectTemplate | String | Διαδρομή προς το πρότυπο για τη δημιουργία έργου από |
| options | PrimaveraReadOptions | η καθορισμένη παρουσία της [`PrimaveraReadOptions`](../../primaverareadoptions/) κλάσης. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε ένα έργο από αρχείο Primavera XML ή Primavera XER που περιέχει πολλαπλά έργα χρησιμοποιώντας τις επιλογές ανάγνωσης Primavera.

```csharp
var options = new PrimaveraReadOptions()
{
    ProjectUid = 4557
};

// Επιστρέφει έργο με ειδικό UID
var project = new Project(DataDir + "Project.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Δείτε επίσης

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(DbSettings) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της [`Project`](../) κλάσης για την ανάγνωση δεδομένων από μια βάση δεδομένων που καθορίζεται από την παρουσία της [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/) κλάσης.

```csharp
public Project(DbSettings settings)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| settings | DbSettings | η καθορισμένη παρουσία της [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/) κλάσης. |

## Παραδείγματα

Δείχνει πώς να εισάγετε ένα έργο από μια βάση δεδομένων Primavera χρησιμοποιώντας τις ρυθμίσεις βάσης δεδομένων.

```csharp
var sb = new SqlConnectionStringBuilder
{
    DataSource = "192.168.56.3,1433",
    Encrypt = true,
    TrustServerCertificate = true,
    InitialCatalog = "PrimaveraEDB",
    NetworkLibrary = "DBMSSOCN",
    UserID = "privuser",
    Password = "***",
};

// Αρχικοποιήστε μια νέα παρουσία της κλάσης PrimaveraDbSettings με τη συμβολοσειρά σύνδεσης και το id του έργου
var settings = new PrimaveraDbSettings(sb.ConnectionString, 4502);

// Αρχικοποιήστε μια νέα παρουσία της κλάσης Project
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Δείτε επίσης

* class [DbSettings](../../../aspose.tasks.connectivity/dbsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, ParseErrorCallback) {#constructor_4}

Αρχικοποιεί μια νέα παρουσία της [`Project`](../) κλάσης από ένα πρότυπο (υπάρχον αρχείο mpp ή mpt).

```csharp
public Project(Stream stream, ParseErrorCallback parseErrorHandler)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | Ροή | Ροή από την οποία θα φορτωθεί ένα πρότυπο. |
| parseErrorHandler | ParseErrorCallback | η καθορισμένη μέθοδος callback για το χειρισμό σφαλμάτων ανάλυσης xml. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε ένα έργο από αρχείο XML με μη έγκυρους χαρακτήρες.

```csharp
public static void LoadProjectFromStream(string brokenXmlData)
{
    // ανοίξτε τη ροή που περιέχει XML με κατεστραμμένα χρονικά διαστήματα
    byte[] bytes = Encoding.UTF8.GetBytes(brokenXmlData);
    using (var stream = new MemoryStream(bytes))
    {
        var project = new Project(stream, CustomDurationHandlerForStream2);
        Console.WriteLine(project.Get(Prj.Name));
    }
}

public static object CustomDurationHandlerForStream2(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Debug.Print("Object field : {0}, Invalid value : {1}", args.FieldName, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var newValue = Duration.ParseTimeSpan(duration);
    Debug.Print("New value : {0}", newValue);
    return newValue;
}
```

### Δείτε επίσης

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, string) {#constructor_6}

Αρχικοποιεί μια νέα παρουσία της [`Project`](../) κλάσης από ένα πρότυπο (υπάρχον αρχείο mpp ή mpt).

```csharp
public Project(Stream stream, string protectionPassword)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | Ροή | Ροή από την οποία θα φορτωθεί ένα πρότυπο. |
| protectionPassword | String | Κωδικός προστασίας. |

## Παρατηρήσεις

Η ανάγνωση αρχείων προστατευμένων με κωδικό υποστηρίζεται επί του παρόντος μόνο για τη μορφή αρχείου MSP 2003.

## Παραδείγματα

Δείχνει πώς να ελέγξετε αν το MPP είναι προστατευμένο με κωδικό.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "PasswordProtected.mpp");
Console.WriteLine("Is file password protected?:" + info.IsPasswordProtected);
```

Δείχνει πώς να διαβάσετε αρχεία MPP προστατευμένα με κωδικό από μια ροή.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var project = new Project(stream, "password");
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, LoadOptions) {#constructor_9}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Project`](../) από ένα πρότυπο (υπάρχον αρχείο mpp ή mpt) με την καθορισμένη παρουσία της κλάσης [`LoadOptions`](../../loadoptions/).

```csharp
public Project(string projectTemplate, LoadOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| projectTemplate | String | Διαδρομή προς το πρότυπο για τη δημιουργία έργου από |
| options | LoadOptions | η καθορισμένη παρουσία της κλάσης [`LoadOptions`](../../loadoptions/). |

## Παραδείγματα

Δείχνει πώς να φορτώσετε το έργο από ένα αρχείο χρησιμοποιώντας την παρουσία &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt;.

```csharp
var options = new LoadOptions
{
    Password = "password"
};
var project = new Project(DataDir + "PasswordProtectedProject.mpp", options);
Console.WriteLine(project.Get(Prj.Name));
```

Δείχνει πώς να διαβάσετε ένα έργο από αρχείο Primavera XML με σφάλμα ανάλυσης.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};

var loadOptions = new LoadOptions()
{
    PrimaveraReadOptions = options,
    ErrorHandler = CustomDurationHandlerForFile
};

// Επιστρέφει έργο με ειδικό UID
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

### Δείτε επίσης

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, LoadOptions) {#constructor_3}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Project`](../) από τη Ροή με την καθορισμένη παρουσία της κλάσης [`LoadOptions`](../../loadoptions/).

```csharp
public Project(Stream stream, LoadOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | Ροή | Ροή του Project Streamclass |
| options | LoadOptions | η καθορισμένη παρουσία της κλάσης [`LoadOptions`](../../loadoptions/) |

## Παραδείγματα

Δείχνει πώς να φορτώσετε το έργο από μια ροή χρησιμοποιώντας την παρουσία &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt;.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Δείτε επίσης

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


