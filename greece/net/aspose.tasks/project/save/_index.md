---
title: "Project.Save"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Project μέθοδος. Αποθηκεύει το έγγραφο σε αρχείο χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης"
type: docs
weight: 1200
url: /el/net/aspose.tasks/project/save/
---
## Save(string, SimpleSaveOptions) {#save_4}

Αποθηκεύει το έγγραφο σε αρχείο χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης.

```csharp
public void Save(string filename, SimpleSaveOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα αρχείου | String | Το όνομα αρχείου. |
| επιλογές | SimpleSaveOptions | Οι επιλογές αποθήκευσης. |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε το project ως αρχείο MPP.

```csharp
var project = new Project();
SimpleSaveOptions options = new MPPSaveOptions();
project.Save(OutDir + "EmptyProjectSaveStream_out.xml", options);
```

### Δείτε επίσης

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string, SaveFileFormat) {#save_3}

Αποθηκεύει τα δεδομένα του έργου στο αρχείο.

```csharp
public void Save(string filename, SaveFileFormat format)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα αρχείου | String | Το όνομα αρχείου. |
| μορφή | SaveFileFormat | Η μορφή αρχείου αποθήκευσης. |

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε ένα έργο και να το αποθηκεύσετε σε μορφή MPP χωρίς να περάσετε αρχείο προτύπου MPP.

```csharp
var project = new Project();

// Το έργο θα αποθηκευτεί σε MPP χρησιμοποιώντας το εσωτερικό πρότυπο MPP.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string) {#save_2}

Αποθηκεύει τα δεδομένα του έργου στο αρχείο σε μορφή mpp.

```csharp
public void Save(string filename)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα αρχείου | String | Το όνομα αρχείου. |

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SimpleSaveOptions) {#save_1}

Αποθηκεύει το έργο σε μια ροή χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης.

```csharp
public void Save(Stream stream, SimpleSaveOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | Ροή | Η ροή. |
| επιλογές | SimpleSaveOptions | Οι επιλογές αποθήκευσης. |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε το project σε ροή ως αρχείο MPP χρησιμοποιώντας τις επιλογές αποθήκευσης MPP.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project();
    SimpleSaveOptions options = new MPPSaveOptions();

    // χρησιμοποιώντας το MPPSaveOptions το αποθηκεύουμε σε μορφή MPP
    project.Save(stream, options);
}
```

Δείχνει πώς να αποθηκεύσετε το project σε ροή ως εικόνα και να ελέγξετε τις επιλογές εικόνας.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // χρησιμοποιώντας το ImageSaveOptions αποθηκεύουμε το έργο σε μορφή εικόνας
    project.Save(stream, options);
}
```

### Δείτε επίσης

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SaveFileFormat) {#save}

Αποθηκεύει τα δεδομένα του έργου στη ροή.

```csharp
public void Save(Stream stream, SaveFileFormat format)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | Ροή | Η ροή. |
| format | SaveFileFormat | η καθορισμένη μορφή αρχείου αποθήκευσης.[`SaveFileFormat`](../../../aspose.tasks.saving/savefileformat/) |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε το project σε ροή ως αρχείο XML MS Project.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    // Γράψτε τη ροή σε μορφή XML
    project.Save(stream, SaveFileFormat.Xml);
}
```

### Δείτε επίσης

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


