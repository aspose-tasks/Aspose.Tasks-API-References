---
title: "枚举 PdfDigitalSignatureHashAlgorithm"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.PdfDigitalSignatureHashAlgorithm 枚举。指定数字签名使用的数字哈希算法"
type: docs
weight: 2090
url: /zh/net/aspose.tasks.saving/pdfdigitalsignaturehashalgorithm/
---
## PdfDigitalSignatureHashAlgorithm enumeration

指定数字签名使用的数字哈希算法。

```csharp
public enum PdfDigitalSignatureHashAlgorithm
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Sha1 | `0` | 指定数字签名使用的数字哈希算法。 |
| Sha256 | `1` | 指定数字签名使用的数字哈希算法。 |
| Sha384 | `2` | 指定数字签名使用的数字哈希算法。 |
| Sha512 | `3` | 指定数字签名使用的数字哈希算法。 |
| Md5 | `4` | 指定数字签名使用的数字哈希算法。 |

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


