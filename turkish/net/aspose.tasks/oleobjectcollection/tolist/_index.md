---
title: "OleObjectCollection.ToList"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "OleObjectCollection yöntemi. OleObjectCollection sınıfının örneğini, OleObject sınıfının örneklerini içeren bir listeye dönüştürür."
type: docs
weight: 30
url: /tr/net/aspose.tasks/oleobjectcollection/tolist/
---
## OleObjectCollection.ToList method

[`OleObjectCollection`](../) sınıfının örneğini, [`OleObject`](../../oleobject/) sınıfının örneklerini içeren bir listeye dönüştürür.

```csharp
public List<OleObject> ToList()
```

### Dönüş Değeri

Listeye dönüştürülen [`OleObjectCollection`](../) sınıfının örneği, [`OleObject`](../../oleobject/) sınıfının örneklerini içerir.

## Örnekler

OLE nesnelerinin koleksiyonuyla nasıl çalışılacağını gösterir.

```csharp
IDictionary<string, string> extensions = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

// indeks erişimi kullanarak
// List<OleObject> list = project.OleObjects.ToList();
// for (var index = 0; index < list.Count; index++)
// {
// var oleObject = list[index];
// }

// veya sayım, OLE nesneleri üzerinde yineleme yapılabilir
foreach (var oleObject in project.OleObjects)
{
    if (string.IsNullOrEmpty(oleObject.FileFormat) || !extensions.ContainsKey(oleObject.FileFormat))
    {
        continue;
    }

    var path = OutDir + "EmbeddedContent_" + extensions[oleObject.FileFormat];
    using (var stream = new FileStream(path, FileMode.Create))
    {
        stream.Write(oleObject.Content, 0, oleObject.Content.Length);
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


