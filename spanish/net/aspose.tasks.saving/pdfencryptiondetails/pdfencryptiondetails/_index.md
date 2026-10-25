---
title: "PdfEncryptionDetails.PdfEncryptionDetails"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de PdfEncryptionDetails. Inicializa una nueva instancia de la clase PdfEncryptionDetails"
type: docs
weight: 10
url: /es/net/aspose.tasks.saving/pdfencryptiondetails/pdfencryptiondetails/
---
## PdfEncryptionDetails constructor

Inicializa una nueva instancia de la clase [`PdfEncryptionDetails`](../).

```csharp
public PdfEncryptionDetails(string userPassword, string ownerPassword, 
    PdfEncryptionAlgorithm encryptionAlgorithm)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| userPassword | Cadena | La contraseña de usuario que permite abrir documentos protegidos. |
| ownerPassword | Cadena | La contraseña del propietario que permite abrir documentos protegidos. |
| encryptionAlgorithm | PdfEncryptionAlgorithm | La instancia de [`PdfEncryptionAlgorithm`](../../pdfencryptionalgorithm/) que indica el algoritmo de cifrado. |

## Ejemplos

Muestra cómo especificar los detalles de cifrado PDF al guardar un proyecto como archivo PDF.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// especifica los detalles de cifrado
var encryptionDetails = new PdfEncryptionDetails(
    // especificar la contraseña del usuario
    "userPassword", 
    // especificar la contraseña del propietario
    "ownerPassword", 
    // especificar el algoritmo de cifrado
    PdfEncryptionAlgorithm.RC4_128);

// especificar los permisos
encryptionDetails.Permissions = PdfPermissions.ModifyContents | PdfPermissions.ModifyAnnotations;

// mostrar las contraseñas del usuario y del propietario
Console.WriteLine("User Password: " + encryptionDetails.UserPassword);
Console.WriteLine("Owner Password: " + encryptionDetails.OwnerPassword);
// mostrar modo de cifrado: RC4_40 o RC4_128
Console.WriteLine("Encryption Algorithm: " + encryptionDetails.EncryptionAlgorithm);
Console.WriteLine("Permissions: " + encryptionDetails.Permissions);

var options = new PdfSaveOptions
{
    EncryptionDetails = encryptionDetails
};

// guardar el proyecto con los detalles de cifrado especificados
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### Ver también

* enum [PdfEncryptionAlgorithm](../../pdfencryptionalgorithm/)
* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


