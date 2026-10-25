---
title: "PdfEncryptionDetails.OwnerPassword"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PdfEncryptionDetails 属性。获取或设置所有者密码"
type: docs
weight: 30
url: /zh/net/aspose.tasks.saving/pdfencryptiondetails/ownerpassword/
---
## PdfEncryptionDetails.OwnerPassword property

获取或设置所有者密码。

```csharp
public string OwnerPassword { get; set; }
```

## 备注

使用正确的所有者密码打开文档（假设它不同于用户密码）可获得对文档的完整（所有者）访问权限。此无限制访问包括更改文档密码和访问权限的能力。

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

* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


