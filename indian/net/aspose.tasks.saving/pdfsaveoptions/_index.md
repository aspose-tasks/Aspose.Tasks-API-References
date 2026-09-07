---
title: "क्लास PdfSaveOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Saving.PdfSaveOptions क्लास। प्रोजेक्ट पेजों को PDF में रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है"
type: docs
weight: 2130
url: /hi/net/aspose.tasks.saving/pdfsaveoptions/
---
## PdfSaveOptions class

PDF में प्रोजेक्ट पेज रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।

```csharp
public class PdfSaveOptions : SaveOptions
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | एक नया `PdfSaveOptions` क्लास का इंस्टेंस इनिशियलाइज़ करता है जिसका उपयोग दस्तावेज़ को [`PDF`](../savefileformat/) फ़ॉर्मेट में सहेजने के लिए किया जा सकता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | प्रोजेक्ट व्यू में दिखाई देने वाली [`BarStyle`](../../aspose.tasks.visualization/barstyle/) क्लास की इंस्टेंस की सूची को प्राप्त करता है या सेट करता है। |
| [Compliance](../../aspose.tasks.saving/pdfsaveoptions/compliance/) { get; set; } | जनरेटेड PDF दस्तावेज़ के लिए वांछित अनुपालन स्तर प्राप्त करता है या सेट करता है। डिफ़ॉल्ट Pdf15 है। |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | कस्टम पेज आकार को पॉइंट्स में प्राप्त करता है या सेट करता है (1 पॉइंट = इंच का 1/72)। |
| [DigitalSignatureDetails](../../aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/) { get; set; } | डिजिटल सिग्नेचर विवरण प्राप्त करता है या सेट करता है। यदि सेट नहीं किया गया, तो कोई साइनिंग नहीं होगी। |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि गैर-कार्य समय को चित्रित किया जाना चाहिए या नहीं (डिफ़ॉल्ट मान TRUE है)। |
| [EncryptionDetails](../../aspose.tasks.saving/pdfsaveoptions/encryptiondetails/) { get; set; } | एन्क्रिप्शन विवरण प्राप्त करता है या सेट करता है। यदि सेट नहीं किया गया, तो कोई एन्क्रिप्शन नहीं किया जाएगा। |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | रेंडरिंग समाप्त करने की तिथि प्राप्त करता है या सेट करता है। |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि पंक्ति की ऊँचाई को उसकी सामग्री के अनुसार बढ़ाया जाना चाहिए या नहीं। |
| [FontSettings](../../aspose.tasks.saving/pdfsaveoptions/fontsettings/) { get; } | प्रोजेक्ट के दृश्य को रेंडर करने के समय उपयोग किए जाने वाले फ़ॉन्ट सेटिंग्स को निर्दिष्ट करता है। |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | प्रोजेक्ट व्यू में दिखाई देने वाले [`Gridline`](../../aspose.tasks.visualization/gridline/) की सूची प्राप्त करता है या सेट करता है। |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि पेज अभिविन्यास पोर्ट्रेट है; यदि पेज अभिविन्यास लैंडस्केप है तो false लौटाता है। |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो परिभाषित करता है कि लेजेंड कैसे रेंडर किया जाए। डिफ़ॉल्ट मान LegendDrawingOptions.OnEveryPage है। |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | PageLegendItem की एक एरे प्राप्त करता है या सेट करता है जो निर्धारित करता है कि पेज लेजेंड में कौन से बार रेंडर किए जाएँ। यदि null है, तो डिफ़ॉल्ट आइटम रेंडर होते हैं। |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि महत्वपूर्ण कार्यों को लाल रंग में दिखाया जाए या नहीं (डिफ़ॉल्ट मान FALSE है)। |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | गैर-कार्य समय का रंग प्राप्त करता है या सेट करता है। |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | प्रोजेक्ट के पृष्ठों की संख्या प्राप्त करता है या सेट करता है। |
| [Pages](../../aspose.tasks.saving/pdfsaveoptions/pages/) { get; set; } | प्रोजेक्ट लेआउट को अलग फ़ाइलों में सहेजते समय सहेजने के लिए पेज नंबरों की सूची प्राप्त करता है या सेट करता है। यदि यह सूची खाली है तो सभी पेज सहेजे जाएंगे। |
| [PageSavingCallback](../../aspose.tasks.saving/pdfsaveoptions/pagesavingcallback/) { get; set; } | एक यूज़र-डिफाइंड कॉलबैक प्राप्त करता है या सेट करता है जिसका उपयोग प्रत्येक रेंडर किए गए पेज के लिए आउटपुट स्ट्रीम प्राप्त करने में किया जाता है। यह तब लागू होता है जब [`SaveToSeparateFiles`](./savetoseparatefiles/) विकल्प उपयोग किया जाता है। |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | रेंडर किए जाने वाले पेज का आकार प्राप्त करता है या सेट करता है (डिफ़ॉल्ट मान PageSize.A4 है)। |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | दस्तावेज़ को सहेजने के लिए उपयोग किए जाने वाले [`PresentationFormat`](../saveoptions/presentationformat/) को प्राप्त करता है या सेट करता है। |
| [ReduceFooterGap](../../aspose.tasks.saving/pdfsaveoptions/reducefootergap/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि अंतिम कार्य और फुटर के बीच का अंतराल घटाया जाना चाहिए या नहीं। |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि ग्राफ़िकल फ़ॉर्मेट में प्रोजेक्ट सहेजते समय प्रोजेक्ट को एक ही पेज पर रेंडर किया जाए या नहीं। पेज आकार बदल दिया जाएगा ताकि रेंडर किया गया प्रोजेक्ट एक पेज में फिट हो सके। |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि सारांश कार्य बार पर उप‑कार्य को चिह्नित किया जाए या नहीं। उप‑कार्य के लिए, Rollup फ़ील्ड यह दर्शाता है कि उप‑कार्य के गैंट बार की जानकारी सारांश कार्य बार में रोल‑अप होगी या नहीं। सारांश कार्यों के लिए, Rollup फ़ील्ड यह दर्शाता है कि सारांश कार्य बार रोल‑अप बार दिखाता है या नहीं। किसी भी उप‑कार्य को उनके पास रोल‑अप करने के लिए आपको सारांश कार्यों के लिए Rollup फ़ील्ड को Yes पर सेट करना आवश्यक है। |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | यदि इस सहेजने विकल्प वस्तु का उपयोग किया जाता है तो दस्तावेज़ को सहेजने के लिए उपयोग किए जाने वाले स्वरूप को प्राप्त करता है या सेट करता है। |
| [SaveToSeparateFiles](../../aspose.tasks.saving/pdfsaveoptions/savetoseparatefiles/) { get; set; } | प्रोजेक्ट पेजों को अलग फ़ाइलों में सहेजने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | रेंडरिंग शुरू करने की तिथि को प्राप्त करता है या सेट करता है। |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | एक कॉलबैक को प्राप्त करता है या सेट करता है जिसका उपयोग कार्य लिंक रेंडरिंग के कुछ पहलुओं को अनुकूलित करने के लिए किया जा सकता है। |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gantt चार्ट और टास्क शीट चार्ट पर कार्यों को क्रमबद्ध करने के लिए तुलना करने वाले को प्राप्त करता है या सेट करता है। |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gantt, टास्क शीट और टास्क उपयोग चार्ट पर रेंडर किए गए कार्यों को फ़िल्टर करने के लिए उपयोग की जाने वाली शर्त को प्राप्त करता है या सेट करता है। |
| [TextCompression](../../aspose.tasks.saving/pdfsaveoptions/textcompression/) { get; set; } | इमेज़ को छोड़कर सभी कंटेंट स्ट्रीम्स के लिए उपयोग किए जाने वाले कम्प्रेशन प्रकार को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट Flate है। |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | प्रोजेक्ट व्यू के रेंडरिंग के दौरान लागू होने वाले टेक्स्ट शैलियों की सूची को प्राप्त करता है या सेट करता है। |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | प्रोजेक्ट को ग्राफिकल फ़ॉर्मेट में सहेजते समय टाइमस्केल (यदि मौजूद हो) को कैसे रेंडर किया जाता है, इसे नियंत्रित करने के लिए उपयोग किए जाने वाले [`Timescale`](../saveoptions/timescale/) मान को प्राप्त करता है या सेट करता है। |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | टाइमस्केल के दाएँ अंत को पृष्ठ के अंत के साथ संरेखित करने के तरीके को परिभाषित करने वाले व्यवहार को प्राप्त करता है या सेट करता है। |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | गैंट चार्ट को रेंडर करते समय ग्रेडिएंट ब्रश का उपयोग किया जाना चाहिए या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | रेंडर करने के लिए व्यू कॉलम की सूची को प्राप्त करता है या सेट करता है ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/))। यदि सेट नहीं किया गया तो केवल कार्य आईडी, कार्य नाम, प्रारंभ और समाप्ति रेंडर होते हैं। यदि View और [`ViewSettings`](../saveoptions/viewsettings/) दोनों गुण सेट हैं, तो View के कॉलम ViewSettings के कॉलम को ओवरराइड करते हैं। |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | रेंडर करने के लिए एक व्यू ([`View`](../saveoptions/view/)) को प्राप्त करता है या सेट करता है। आप इस विकल्प का उपयोग करके स्पष्ट रूप से निर्दिष्ट कर सकते हैं कि कौन सा व्यू PDF, HTML या इमेज फ़ॉर्मेट में सहेजा जाना चाहिए। यदि यह गुण सेट है, तो प्रोजेक्ट सहेजते समय [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) गुण को अनदेखा किया जाता है। व्यू निम्नलिखित स्क्रीन में से किसी एक से होना चाहिए (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

## उदाहरण

दिखाता है कि प्रोजेक्ट के चयनित पेजों को PDF फ़ाइल में कैसे सहेजा जाए।

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// आइए जांचते हैं कि कितने पेज निर्यात किए जा सकते हैं
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### संबंधित देखें

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


