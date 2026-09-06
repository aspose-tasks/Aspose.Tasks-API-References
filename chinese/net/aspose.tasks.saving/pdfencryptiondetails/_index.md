---
title: "类 PdfEncryptionDetails"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.PdfEncryptionDetails 类。包含 PDF 加密的详细信息"
type: docs
weight: 2110
url: /zh/net/aspose.tasks.saving/pdfencryptiondetails/
---
## PdfEncryptionDetails class

包含 PDF 加密的详细信息。

```csharp
public class PdfEncryptionDetails
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PdfEncryptionDetails](pdfencryptiondetails/)(string, string, PdfEncryptionAlgorithm) | 初始化 `PdfEncryptionDetails` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [EncryptionAlgorithm](../../aspose.tasks.saving/pdfencryptiondetails/encryptionalgorithm/) { get; set; } | 获取或设置加密模式。 |
| [OwnerPassword](../../aspose.tasks.saving/pdfencryptiondetails/ownerpassword/) { get; set; } | 获取或设置所有者密码。 |
| [Permissions](../../aspose.tasks.saving/pdfencryptiondetails/permissions/) { get; set; } | 获取或设置权限。 |
| [UserPassword](../../aspose.tasks.saving/pdfencryptiondetails/userpassword/) { get; set; } | 获取或设置用户密码。 |

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


