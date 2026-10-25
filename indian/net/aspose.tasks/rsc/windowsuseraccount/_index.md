---
title: "Rsc.WindowsUserAccount"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। संसाधन से जुड़ा NT खाता"
type: docs
weight: 680
url: /hi/net/aspose.tasks/rsc/windowsuseraccount/
---
## Rsc.WindowsUserAccount field

संसाधन से जुड़ा NT खाता।

```csharp
public static readonly Key<string, RscKey> WindowsUserAccount;
```

## उदाहरण

दिखाता है कि संसाधन की मेटा प्रॉपर्टीज़ कैसे सेट की जाएँ।

```csharp
var project = new Project(DataDir + "Project.mpp");

// संसाधन जोड़ें और संसाधन मेटा डेटा सेट करें
var resource = project.Resources.Add("Rsc 1");
resource.Set(Rsc.EMailAddress, "1@gmail.com");
resource.Set(Rsc.WindowsUserAccount, "user_acc1");
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


