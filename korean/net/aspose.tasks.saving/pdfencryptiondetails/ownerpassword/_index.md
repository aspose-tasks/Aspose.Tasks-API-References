---
title: "PdfEncryptionDetails.OwnerPassword"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PdfEncryptionDetails 속성. 소유자 비밀번호를 가져오거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.saving/pdfencryptiondetails/ownerpassword/
---
## PdfEncryptionDetails.OwnerPassword property

소유자 비밀번호를 가져오거나 설정합니다.

```csharp
public string OwnerPassword { get; set; }
```

## 비고

올바른 소유자 비밀번호(사용자 비밀번호와 다르다고 가정)로 문서를 열면 문서에 대한 전체(소유자) 접근 권한이 부여됩니다. 이 무제한 접근 권한에는 문서의 비밀번호 및 접근 권한을 변경할 수 있는 기능이 포함됩니다.

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

* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


