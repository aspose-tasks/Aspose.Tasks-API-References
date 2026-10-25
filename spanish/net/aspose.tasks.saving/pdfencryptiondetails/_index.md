---
title: "Clase PdfEncryptionDetails"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Saving.PdfEncryptionDetails. Contiene detalles para un cifrado PDF"
type: docs
weight: 2110
url: /es/net/aspose.tasks.saving/pdfencryptiondetails/
---
## PdfEncryptionDetails class

Contiene detalles de un cifrado PDF.

```csharp
public class PdfEncryptionDetails
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PdfEncryptionDetails](pdfencryptiondetails/)(string, string, PdfEncryptionAlgorithm) | Inicializa una nueva instancia de la clase `PdfEncryptionDetails`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [EncryptionAlgorithm](../../aspose.tasks.saving/pdfencryptiondetails/encryptionalgorithm/) { get; set; } | Obtiene o establece el modo de cifrado. |
| [OwnerPassword](../../aspose.tasks.saving/pdfencryptiondetails/ownerpassword/) { get; set; } | Obtiene o establece la contraseña del propietario. |
| [Permissions](../../aspose.tasks.saving/pdfencryptiondetails/permissions/) { get; set; } | Obtiene o establece los permisos. |
| [UserPassword](../../aspose.tasks.saving/pdfencryptiondetails/userpassword/) { get; set; } | Obtiene o establece la contraseña del usuario. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


