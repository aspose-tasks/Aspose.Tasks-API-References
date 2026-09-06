---
title: "类 PdfDigitalSignatureDetails"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.PdfDigitalSignatureDetails 类。包含 PDF 数字签名的详细信息"
type: docs
weight: 2080
url: /zh/net/aspose.tasks.saving/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails class

包含 PDF 数字签名的详细信息。

```csharp
public class PdfDigitalSignatureDetails
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PdfDigitalSignatureDetails](pdfdigitalsignaturedetails/)(X509Certificate2, string, string, DateTime, PdfDigitalSignatureHashAlgorithm) | 初始化 `PdfDigitalSignatureDetails` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Certificate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/certificate/) { get; set; } | 获取或设置用于签名的证书。 |
| [HashAlgorithm](../../aspose.tasks.saving/pdfdigitalsignaturedetails/hashalgorithm/) { get; set; } | 获取或设置哈希算法。 |
| [Location](../../aspose.tasks.saving/pdfdigitalsignaturedetails/location/) { get; set; } | 获取或设置签名位置。 |
| [Reason](../../aspose.tasks.saving/pdfdigitalsignaturedetails/reason/) { get; set; } | 获取或设置签名原因。 |
| [SignatureDate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/signaturedate/) { get; set; } | 获取或设置签名日期。 |

## 备注

目前，数字签署 PDF 文档仅在 .NET 2.0 或更高版本可用。

## 示例

展示如何使用 PDF 数字签名详细信息。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new PdfSaveOptions();

var certificate = new X509Certificate2();

// 创建 PDF 签名详细信息
var signatureDetails = new PdfDigitalSignatureDetails(
    // 指定证书
    certificate, 
    // 指定签名原因
    "reason",
    // 指定签名位置
    "location", 
    // 指定签名日期
    new DateTime(2019, 1, 1), 
    // 指定签名的哈希算法
    PdfDigitalSignatureHashAlgorithm.Sha1);

Console.WriteLine("Certificate: " + signatureDetails.Certificate);
Console.WriteLine("Reason: " + signatureDetails.Reason);
Console.WriteLine("Location: " + signatureDetails.Location);
Console.WriteLine("Signature Date: " + signatureDetails.SignatureDate);
Console.WriteLine("Hash Algorithm: " + signatureDetails.HashAlgorithm);

// 设置数字签名详细信息
options.DigitalSignatureDetails = signatureDetails;

// 使用指定的加密详细信息保存项目
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### 另见

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


