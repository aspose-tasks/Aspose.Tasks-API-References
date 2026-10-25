---
title: "枚举 PdfEncryptionAlgorithm"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.PdfEncryptionAlgorithm 枚举。指定用于加密 PDF 文档的加密算法"
type: docs
weight: 2100
url: /zh/net/aspose.tasks.saving/pdfencryptionalgorithm/
---
## PdfEncryptionAlgorithm enumeration

指定用于加密 PDF 文档的加密算法。

```csharp
public enum PdfEncryptionAlgorithm
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| RC4_40 | `0` | 指定用于加密 PDF 文档的加密算法。 |
| RC4_128 | `1` | 指定用于加密 PDF 文档的加密算法。 |

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


