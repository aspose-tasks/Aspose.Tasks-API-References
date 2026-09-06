---
title: "Project.Save"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 方法。使用指定的保存选项将文档保存到文件中"
type: docs
weight: 1200
url: /zh/net/aspose.tasks/project/save/
---
## Save(string, SimpleSaveOptions) {#save_4}

使用指定的保存选项将文档保存到文件。

```csharp
public void Save(string filename, SimpleSaveOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件名 | 字符串 | 文件名。 |
| 选项 | SimpleSaveOptions | 保存选项。 |

## 示例

展示如何将项目保存为 MPP 文件。

```csharp
var project = new Project();
SimpleSaveOptions options = new MPPSaveOptions();
project.Save(OutDir + "EmptyProjectSaveStream_out.xml", options);
```

### 另见

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string, SaveFileFormat) {#save_3}

将项目数据保存到文件。

```csharp
public void Save(string filename, SaveFileFormat format)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件名 | 字符串 | 文件名。 |
| 格式 | SaveFileFormat | 保存文件格式。 |

## 示例

展示如何创建项目并保存为 MPP 格式，而无需提供 MPP 模板文件。

```csharp
var project = new Project();

// 项目将使用内部 MPP 模板保存为 MPP。
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string) {#save_2}

以 mpp 格式将项目数据保存到文件。

```csharp
public void Save(string filename)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件名 | 字符串 | 文件名。 |

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SimpleSaveOptions) {#save_1}

使用指定的保存选项将项目保存到流中。

```csharp
public void Save(Stream stream, SimpleSaveOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 流。 |
| 选项 | SimpleSaveOptions | 保存选项。 |

## 示例

展示如何使用 MPP 保存选项将项目保存到流中为 MPP 文件。

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project();
    SimpleSaveOptions options = new MPPSaveOptions();

    // 通过使用 MPPSaveOptions，我们将其保存为 MPP 格式
    project.Save(stream, options);
}
```

展示如何将项目保存到流中为图像并控制图像选项。

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // 通过使用 ImageSaveOptions，我们将项目保存为图像格式
    project.Save(stream, options);
}
```

### 另见

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SaveFileFormat) {#save}

将项目数据保存到流中。

```csharp
public void Save(Stream stream, SaveFileFormat format)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 流。 |
| format | SaveFileFormat | 指定的保存文件格式。[`SaveFileFormat`](../../../aspose.tasks.saving/savefileformat/) |

## 示例

展示如何将项目保存到流中为 XML MS Project 文件。

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    // 将流写入 XML 格式
    project.Save(stream, SaveFileFormat.Xml);
}
```

### 另见

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


