---
title: "Project.Save"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Project. Enregistre le document dans un fichier en utilisant les options d’enregistrement spécifiées"
type: docs
weight: 1200
url: /fr/net/aspose.tasks/project/save/
---
## Save(string, SimpleSaveOptions) {#save_4}

Enregistre le document dans un fichier en utilisant les options d’enregistrement spécifiées.

```csharp
public void Save(string filename, SimpleSaveOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| nom de fichier | Chaîne | Le nom du fichier. |
| options | SimpleSaveOptions | Les options d’enregistrement. |

## Exemples

Montre comment enregistrer le projet en tant que fichier MPP.

```csharp
var project = new Project();
SimpleSaveOptions options = new MPPSaveOptions();
project.Save(OutDir + "EmptyProjectSaveStream_out.xml", options);
```

### Voir aussi

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string, SaveFileFormat) {#save_3}

Enregistre les données du projet dans le fichier.

```csharp
public void Save(string filename, SaveFileFormat format)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| nom de fichier | Chaîne | Le nom du fichier. |
| format | SaveFileFormat | Le format du fichier d’enregistrement. |

## Exemples

Montre comment créer un projet et l'enregistrer au format MPP sans fournir de fichier de modèle MPP.

```csharp
var project = new Project();

// Le projet sera enregistré au format MPP en utilisant le modèle MPP interne.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string) {#save_2}

Enregistre les données du projet dans le fichier au format mpp.

```csharp
public void Save(string filename)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| nom de fichier | Chaîne | Le nom du fichier. |

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SimpleSaveOptions) {#save_1}

Enregistre le projet dans un flux en utilisant les options d’enregistrement spécifiées.

```csharp
public void Save(Stream stream, SimpleSaveOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flux | Flux | Le flux. |
| options | SimpleSaveOptions | Les options d’enregistrement. |

## Exemples

Montre comment enregistrer le projet dans un flux en tant que fichier MPP en utilisant les options d’enregistrement MPP.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project();
    SimpleSaveOptions options = new MPPSaveOptions();

    // en utilisant MPPSaveOptions, nous l’enregistrons au format MPP
    project.Save(stream, options);
}
```

Montre comment enregistrer le projet dans un flux en tant qu’image et contrôler les options d’image.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // en utilisant ImageSaveOptions, nous enregistrons le projet au format image
    project.Save(stream, options);
}
```

### Voir aussi

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SaveFileFormat) {#save}

Enregistre les données du projet dans le flux.

```csharp
public void Save(Stream stream, SaveFileFormat format)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flux | Flux | Le flux. |
| format | SaveFileFormat | le format de fichier d’enregistrement spécifié.[`SaveFileFormat`](../../../aspose.tasks.saving/savefileformat/) |

## Exemples

Montre comment enregistrer le projet dans un flux en tant que fichier XML MS Project.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    // Écrire le flux au format XML
    project.Save(stream, SaveFileFormat.Xml);
}
```

### Voir aussi

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


