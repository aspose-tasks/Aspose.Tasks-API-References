---
title: "枚举 PdfPermissions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.PdfPermissions 枚举。指定用于访问 PDF 文档的权限"
type: docs
weight: 2120
url: /zh/net/aspose.tasks.saving/pdfpermissions/
---
## PdfPermissions enumeration

指定访问 PDF 文档时使用的权限。

```csharp
public enum PdfPermissions
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `0` | 指定访问 PDF 文档时使用的权限。 |
| Printing | `4` | 指定访问 PDF 文档时使用的权限。 |
| ModifyContents | `8` | 指定访问 PDF 文档时使用的权限。 |
| ContentCopy | `16` | 指定访问 PDF 文档时使用的权限。 |
| ModifyAnnotations | `32` | 指定访问 PDF 文档时使用的权限。 |
| FillIn | `256` | 指定访问 PDF 文档时使用的权限。 |
| ContentCopyForAccessibility | `512` | 指定访问 PDF 文档时使用的权限。 |
| DocumentAssembly | `1024` | 指定访问 PDF 文档时使用的权限。 |
| HighResolutionPrinting | `2052` | 指定访问 PDF 文档时使用的权限。 |
| AllowAll | `65535` | 指定访问 PDF 文档时使用的权限。 |

## 示例

展示在将项目保存为 PDF 文件时如何指定 PDF 加密详细信息。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// 让我们指定加密详细信息
var encryptionDetails = new PdfEncryptionDetails(
    // 指定用户密码
    "userPassword", 
    // 指定所有者密码
    "ownerPassword", 
    // 指定加密算法
    PdfEncryptionAlgorithm.RC4_128);

// 指定权限
encryptionDetails.Permissions = PdfPermissions.ModifyContents | PdfPermissions.ModifyAnnotations;

// 显示用户和所有者密码
Console.WriteLine("User Password: " + encryptionDetails.UserPassword);
Console.WriteLine("Owner Password: " + encryptionDetails.OwnerPassword);
// 显示加密模式：RC4_40 或 RC4_128
Console.WriteLine("Encryption Algorithm: " + encryptionDetails.EncryptionAlgorithm);
Console.WriteLine("Permissions: " + encryptionDetails.Permissions);

var options = new PdfSaveOptions
{
    EncryptionDetails = encryptionDetails
};

// 使用指定的加密详细信息保存项目
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### 另见

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


