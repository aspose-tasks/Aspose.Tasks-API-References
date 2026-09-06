---
title: "PdfEncryptionDetails.UserPassword"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PdfEncryptionDetails 属性。获取或设置用户密码"
type: docs
weight: 50
url: /zh/net/aspose.tasks.saving/pdfencryptiondetails/userpassword/
---
## PdfEncryptionDetails.UserPassword property

获取或设置用户密码。

```csharp
public string UserPassword { get; set; }
```

## 备注

使用正确的用户密码打开文档（或打开没有用户密码的文档）可根据文档加密字典中指定的用户访问权限执行额外操作。

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


