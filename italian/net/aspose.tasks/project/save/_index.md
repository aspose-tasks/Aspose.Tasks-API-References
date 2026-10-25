---
title: "Project.Save"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Project. Salva il documento in un file utilizzando le opzioni di salvataggio specificate"
type: docs
weight: 1200
url: /it/net/aspose.tasks/project/save/
---
## Save(string, SimpleSaveOptions) {#save_4}

Salva il documento in un file utilizzando le opzioni di salvataggio specificate.

```csharp
public void Save(string filename, SimpleSaveOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nomefile | Stringa | Il nome del file. |
| opzioni | SimpleSaveOptions | Le opzioni di salvataggio. |

## Esempi

Mostra come salvare il progetto come file MPP.

```csharp
var project = new Project();
SimpleSaveOptions options = new MPPSaveOptions();
project.Save(OutDir + "EmptyProjectSaveStream_out.xml", options);
```

### Vedi anche

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string, SaveFileFormat) {#save_3}

Salva i dati del progetto nel file.

```csharp
public void Save(string filename, SaveFileFormat format)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nomefile | Stringa | Il nome del file. |
| formato | SaveFileFormat | Il formato del file di salvataggio. |

## Esempi

Mostra come creare un progetto e salvarlo in formato MPP senza fornire un file modello MPP.

```csharp
var project = new Project();

// Il progetto sarà salvato in MPP utilizzando un modello MPP interno.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string) {#save_2}

Salva i dati del progetto nel file in formato mpp.

```csharp
public void Save(string filename)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nomefile | Stringa | Il nome del file. |

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SimpleSaveOptions) {#save_1}

Salva il progetto in uno stream utilizzando le opzioni di salvataggio specificate.

```csharp
public void Save(Stream stream, SimpleSaveOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | Flusso | Il flusso. |
| opzioni | SimpleSaveOptions | Le opzioni di salvataggio. |

## Esempi

Mostra come salvare il progetto in un flusso come file MPP utilizzando le opzioni di salvataggio MPP.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project();
    SimpleSaveOptions options = new MPPSaveOptions();

    // utilizzando MPPSaveOptions lo salviamo in formato MPP
    project.Save(stream, options);
}
```

Mostra come salvare il progetto in un flusso come immagine e controllare le opzioni dell'immagine.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // utilizzando ImageSaveOptions salviamo il progetto in formato immagine
    project.Save(stream, options);
}
```

### Vedi anche

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SaveFileFormat) {#save}

Salva i dati del progetto nello stream.

```csharp
public void Save(Stream stream, SaveFileFormat format)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | Flusso | Il flusso. |
| format | SaveFileFormat | il formato di salvataggio specificato.[`SaveFileFormat`](../../../aspose.tasks.saving/savefileformat/) |

## Esempi

Mostra come salvare il progetto in un flusso come file XML di MS Project.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    // Scrivi il flusso in formato XML
    project.Save(stream, SaveFileFormat.Xml);
}
```

### Vedi anche

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


