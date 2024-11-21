---
title: MPPSaveOptions.ProtectionPassword
second_title: Aspose.Tasks for .NET API Reference
description: MPPSaveOptions property. Gets or sets a password which is used to protect a resulting MPP file. Currently is supported for MS Project 2010 and newer formats. Null value indicates that the project file is not protected
type: docs
weight: 30
url: /net/aspose.tasks.saving/mppsaveoptions/protectionpassword/
---
## MPPSaveOptions.ProtectionPassword property

Gets or sets a password which is used to protect a resulting MPP file. Currently is supported for MS Project 2010 and newer formats. Null value indicates that the project file is not protected.

```csharp
public string ProtectionPassword { get; set; }
```

## Examples

Shows how to save a project to password protected MPP file.

```csharp
try
{

    var project = new Project(DataDir + "Project1.mpp");

    SimpleSaveOptions options = new MPPSaveOptions
    {
        ProtectionPassword = "password!234"
    };

    project.Save(OutDir + "PasswordProtected.mpp", options);
}
catch (NotSupportedException ex)
{
    Console.WriteLine(ex.Message + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
}
```

### See Also

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


