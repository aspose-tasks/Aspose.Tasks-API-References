---
title: Project.Save
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Saves the document to a file using the specified save options
type: docs
weight: 1210
url: /net/aspose.tasks/project/save/
---
## Save(string, SimpleSaveOptions) {#save_4}

Saves the document to a file using the specified save options.

```csharp
public void Save(string filename, SimpleSaveOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filename | String | The file name. |
| options | SimpleSaveOptions | The save options. |

## Examples

Shows how to save project as an MPP file.

```csharp
var project = new Project();
SimpleSaveOptions options = new MPPSaveOptions();
project.Save(OutDir + "EmptyProjectSaveStream_out.xml", options);
```

### See Also

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string, SaveFileFormat) {#save_3}

Saves the project data to the file.

```csharp
public void Save(string filename, SaveFileFormat format)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filename | String | The file name. |
| format | SaveFileFormat | The save file format. |

## Examples

Shows how to create a project and save it into MPP format without passing of an MPP template file.

```csharp
var project = new Project();

// The project will be saved into MPP by using internal MPP template.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string) {#save_2}

Saves the project data to the file in mpp format.

```csharp
public void Save(string filename)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filename | String | The file name. |

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SimpleSaveOptions) {#save_1}

Saves the project to a stream using the specified save options.

```csharp
public void Save(Stream stream, SimpleSaveOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream. |
| options | SimpleSaveOptions | The save options. |

## Examples

Shows how to save project into a stream as an MPP file by using MPP save options.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project();
    SimpleSaveOptions options = new MPPSaveOptions();

    // by using of MPPSaveOptions we save it in MPP format
    project.Save(stream, options);
}
```

Shows how to save project into a stream as an image and to control image options.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // by using of ImageSaveOptions we save the project into image format
    project.Save(stream, options);
}
```

### See Also

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SaveFileFormat) {#save}

Saves the project data to the stream.

```csharp
public void Save(Stream stream, SaveFileFormat format)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream. |
| format | SaveFileFormat | the specified save file format.[`SaveFileFormat`](../../../aspose.tasks.saving/savefileformat/) |

## Examples

Shows how to save project into a stream as an XML MS Project file.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    // Write the stream into XML format
    project.Save(stream, SaveFileFormat.Xml);
}
```

### See Also

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


