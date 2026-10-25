---
title: "PdfDigitalSignatureDetails.PdfDigitalSignatureDetails"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PdfDigitalSignatureDetails 构造函数。初始化 PdfDigitalSignatureDetails 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks.saving/pdfdigitalsignaturedetails/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails constructor

初始化 [`PdfDigitalSignatureDetails`](../) 类的新实例。

```csharp
public PdfDigitalSignatureDetails(X509Certificate2 certificate, string reason, string location, 
    DateTime signatureDate, PdfDigitalSignatureHashAlgorithm hashAlgorithm)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 证书 | X509Certificate2 | 用于签名的 X509Certificate2 实例。 |
| 原因 | 字符串 | 签署的原因。 |
| 位置 | 字符串 | 签署的位置。 |
| 签署日期 | DateTime | 签署的日期。 |
| 哈希算法 | PdfDigitalSignatureHashAlgorithm | 签署的哈希算法。 |

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

* enum [PdfDigitalSignatureHashAlgorithm](../../pdfdigitalsignaturehashalgorithm/)
* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


