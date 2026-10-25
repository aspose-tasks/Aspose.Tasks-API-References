---
title: "열거형 PdfEncryptionAlgorithm"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.PdfEncryptionAlgorithm 열거형. PDF 문서를 암호화하는 데 사용할 암호화 알고리즘을 지정합니다"
type: docs
weight: 2100
url: /ko/net/aspose.tasks.saving/pdfencryptionalgorithm/
---
## PdfEncryptionAlgorithm enumeration

PDF 문서를 암호화하는 데 사용할 암호화 알고리즘을 지정합니다.

```csharp
public enum PdfEncryptionAlgorithm
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| RC4_40 | `0` | PDF 문서를 암호화하는 데 사용할 암호화 알고리즘을 지정합니다. |
| RC4_128 | `1` | PDF 문서를 암호화하는 데 사용할 암호화 알고리즘을 지정합니다. |

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


