---
title: "열거형 PdfPermissions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.PdfPermissions 열거형. PDF 문서에 접근하기 위해 사용할 권한을 지정합니다."
type: docs
weight: 2120
url: /ko/net/aspose.tasks.saving/pdfpermissions/
---
## PdfPermissions enumeration

PDF 문서에 접근하기 위한 권한을 지정합니다.

```csharp
public enum PdfPermissions
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| None | `0` | PDF 문서에 접근하기 위한 권한을 지정합니다. |
| Printing | `4` | PDF 문서에 접근하기 위한 권한을 지정합니다. |
| ModifyContents | `8` | PDF 문서에 접근하기 위한 권한을 지정합니다. |
| ContentCopy | `16` | PDF 문서에 접근하기 위한 권한을 지정합니다. |
| ModifyAnnotations | `32` | PDF 문서에 접근하기 위한 권한을 지정합니다. |
| FillIn | `256` | PDF 문서에 접근하기 위한 권한을 지정합니다. |
| ContentCopyForAccessibility | `512` | PDF 문서에 접근하기 위한 권한을 지정합니다. |
| DocumentAssembly | `1024` | PDF 문서에 접근하기 위한 권한을 지정합니다. |
| HighResolutionPrinting | `2052` | PDF 문서에 접근하기 위한 권한을 지정합니다. |
| AllowAll | `65535` | PDF 문서에 접근하기 위한 권한을 지정합니다. |

## 예제

프로젝트를 PDF 파일로 저장할 때 PDF 암호화 세부 정보를 지정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// 암호화 세부 정보를 지정해 보세요
var encryptionDetails = new PdfEncryptionDetails(
    // 사용자 비밀번호 지정
    "userPassword", 
    // 소유자 비밀번호 지정
    "ownerPassword", 
    // 암호화 알고리즘 지정
    PdfEncryptionAlgorithm.RC4_128);

// 권한 지정
encryptionDetails.Permissions = PdfPermissions.ModifyContents | PdfPermissions.ModifyAnnotations;

// 사용자 및 소유자 비밀번호 표시
Console.WriteLine("User Password: " + encryptionDetails.UserPassword);
Console.WriteLine("Owner Password: " + encryptionDetails.OwnerPassword);
// 암호화 모드 표시: RC4_40 또는 RC4_128
Console.WriteLine("Encryption Algorithm: " + encryptionDetails.EncryptionAlgorithm);
Console.WriteLine("Permissions: " + encryptionDetails.Permissions);

var options = new PdfSaveOptions
{
    EncryptionDetails = encryptionDetails
};

// 지정된 암호화 세부 정보를 사용하여 프로젝트를 저장합니다
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### 또 보기

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


