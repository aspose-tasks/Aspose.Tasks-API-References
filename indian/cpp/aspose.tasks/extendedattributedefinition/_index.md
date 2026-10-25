---
title: "Aspose::Tasks::ExtendedAttributeDefinition क्लास"
linktitle: "ExtendedAttributeDefinition"
articleTitle: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks C++ के लिए"
description: "परियोजना से जुड़ी विस्तारित गुण परिभाषा का प्रतिनिधित्व करता है।"
type: docs
weight: 10
url: /hi/cpp/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

परियोजना से जुड़ी विस्तारित गुण परिभाषा का प्रतिनिधित्व करता है।

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [AddLookupValue](./addlookupvalue/) | आंतरिक लुकअप सूची में एक मान जोड़ता है। यह ValueList . के साथ हेरफेर करने का एक पसंदीदा तरीका है। |
| [CreateExtendedAttribute (7 overloads)](./createextendedattribute/) | एक नया विस्तारित गुण बनाता है जिसमें फ़ील्ड ID इस ऑब्जेक्ट के फ़ील्ड ID मान के बराबर होता है। |
| [CreateLookupResourceDefinition (2 overloads)](./createlookupresourcedefinition/) | लुकअप के साथ एक विस्तारित गुण परिभाषा बनाने वाली फ़ैक्टरी मेथड। इसमें CalculationType Tasks::CalculationType::Lookup के बराबर है और यह केवल Resources में उपयोग की जा सकती है। जब इस मेथड को कॉल करते हैं तो आपको customFieldType , fieldId और alias निर्दिष्ट करने की आवश्यकता है। |
| [CreateLookupTaskDefinition (2 overloads)](./createlookuptaskdefinition/) | लुकअप के साथ एक विस्तारित गुण परिभाषा बनाने वाली फ़ैक्टरी मेथड। इसमें CalculationType Tasks::CalculationType::Lookup के बराबर है और यह केवल Tasks में उपयोग की जा सकती है। जब इस मेथड को कॉल करते हैं तो आपको customFieldType , fieldId और alias निर्दिष्ट करने की आवश्यकता है। |
| [CreateResourceDefinition (2 overloads)](./createresourcedefinition/) | सरल विस्तारित गुण परिभाषा बनाने वाली फ़ैक्टरी मेथड, जिसे Microsoft Project "None" के रूप में दिखाता है। इसमें CalculationType Tasks::CalculationType::None के बराबर है और यह केवल Resource में उपयोग की जा सकती है। जब इस मेथड को कॉल करते हैं तो आपको customFieldType , fieldId और alias निर्दिष्ट करने की आवश्यकता है। |
| [CreateTaskDefinition (2 overloads)](./createtaskdefinition/) | सरल विस्तारित गुण परिभाषा बनाने वाली फ़ैक्टरी मेथड, जिसे Microsoft Project "None" के रूप में दिखाता है। इसमें CalculationType Tasks::CalculationType::None के बराबर है और यह केवल Tasks में उपयोग की जा सकती है। जब इस मेथड को कॉल किया जाता है तो आपको customFieldType , fieldId और alias निर्दिष्ट करने की आवश्यकता है। |
| [Equals](./equals/) | एक फ़्लैग लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [get_Alias](./get_alias/) | कस्टम फ़ील्ड का उपनाम प्राप्त करता है। |
| [get_AppendNewValues](./get_appendnewvalues/) | प्रोजेक्ट में जोड़े गए नए मानों को स्वचालित रूप से सूची में जोड़ने की स्थिति दर्शाने वाला मान प्राप्त करता है। |
| [get_AutoRollDown](./get_autorolldown/) | असाइनमेंट्स में स्वचालित रोल डाउन सक्षम है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_CalculationType](./get_calculationtype/) | कस्टम एट्रिब्यूट मान की गणना प्रकार प्राप्त करता है। |
| [get_CfType](./get_cftype/) | कस्टम फ़ील्ड का प्रकार प्राप्त करता है। |
| [get_Default](./get_default/) | सूची में डिफ़ॉल्ट मान प्राप्त करता है। |
| [get_DefaultGuid](./get_defaultguid/) | डिफ़ॉल्ट लुकअप टेबल एंट्री का Guid प्राप्त करता है। |
| [get_ElementType](./get_elementtype/) | विस्तारित एट्रिब्यूट का कार्य, संसाधन या असाइनमेंट से जुड़ा होना प्राप्त करता है। |
| [get_FieldId](./get_fieldid/) | कस्टम फ़ील्ड के प्रोजेक्ट आईडी के अनुरूप प्राप्त करता है। FieldId प्रॉपर्टी निर्दिष्ट करने के लिए Aspose::Tasks::ExtendedAttributeTask क्लास के एक स्थिरांक की स्ट्रिंग प्रतिनिधित्व का उपयोग करें। |
| [get_FieldName](./get_fieldname/) | कस्टम फ़ील्ड का नाम प्राप्त करता है। |
| [get_Formula](./get_formula/) | Microsoft Project द्वारा कस्टम टास्क फ़ील्ड को भरने के लिए उपयोग किए जाने वाले फ़ॉर्मूला को प्राप्त करता है। |
| [get_GraphicalIndicator](./get_graphicalindicator/) | विस्तारित एट्रिब्यूट से जुड़ी ग्राफ़िकल इंडिकेटर जानकारी प्राप्त करता है। MPP फ़ॉर्मेट पर लागू। |
| [get_Guid](./get_guid/) | कस्टम फ़ील्ड का Guid प्राप्त करता है। |
| [get_LookupUid](./get_lookupuid/) | कस्टम फ़ील्ड से जुड़ी लुकअप टेबल का Guid प्राप्त करता है। |
| [get_MaxMultiValues](./get_maxmultivalues/) | पिक लिस्ट में सेट किए जा सकने वाले अधिकतम मानों की संख्या प्राप्त करता है। |
| [get_ParentProject](./get_parentproject/) | ExtendedAttributeDefinition इंस्टेंस के लिए पैरेंट प्रोजेक्ट प्राप्त करता है। |
| [get_PhoneticsAlias](./get_phoneticsalias/) | कस्टम फ़ील्ड के उपनाम की ध्वन्यात्मक उच्चारण प्राप्त करता है। |
| [get_RestrictValues](./get_restrictvalues/) | कस्टम फ़ील्ड मानों को ValueList में मौजूद मानों तक सीमित करने की स्थिति दर्शाने वाला मान प्राप्त करता है। |
| [get_RollupType](./get_rolluptype/) | रोलअप्स की गणना विधि प्राप्त करता है। |
| [get_SecondaryGuid](./get_secondaryguid/) | विस्तारित एट्रिब्यूट का सेकेंडरी Guid प्राप्त करता है। |
| [get_SecondaryPid](./get_secondarypid/) | कस्टम फ़ील्ड का सेकेंडरी PID प्राप्त करता है। |
| [get_SummaryRowsCalculationType](./get_summaryrowscalculationtype/) | समरी रो के लिए कस्टम एट्रिब्यूट मान की गणना प्रकार प्राप्त करता है। |
| [get_UserDef](./get_userdef/) | कस्टम फ़ील्ड उपयोगकर्ता द्वारा परिभाषित है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_ValueList](./get_valuelist/) | List< Value > ValueList प्राप्त करता है। |
| [get_ValuelistSortOrder](./get_valuelistsortorder/) | वैल्यू लिस्ट की सॉर्टिंग विधि प्राप्त करता है। मान हैं: 0=अवरोही, 1=आरोही। |
| [GetHashCode](./gethashcode/) | ExtendedAttributeDefinition क्लास की इंस्टेंस के लिए हैश कोड लौटाता है। |
| [RemoveLookupValue](./removelookupvalue/) | आंतरिक लुकअप सूची से एक मान हटाता है। यह ValueList के साथ हेरफेर करने का पसंदीदा तरीका है। |
| [set_Alias](./set_alias/) | कस्टम फ़ील्ड का उपनाम सेट करता है। |
| [set_AppendNewValues](./set_appendnewvalues/) | एक मान सेट करता है जो दर्शाता है कि प्रोजेक्ट में जोड़े गए नए मान स्वचालित रूप से सूची में जोड़ें जाएँ। |
| [set_AutoRollDown](./set_autorolldown/) | एक मान सेट करता है जो दर्शाता है कि असाइनमेंट्स में स्वचालित रोल डाउन सक्षम है या नहीं। |
| [set_CalculationType](./set_calculationtype/) | कस्टम एट्रिब्यूट के मान की गणना प्रकार सेट करता है। |
| [set_Default](./set_default/) | सूची में डिफ़ॉल्ट मान सेट करता है। |
| [set_DefaultGuid](./set_defaultguid/) | डिफ़ॉल्ट लुकअप टेबल एंट्री का Guid सेट करता है। |
| [set_ElementType](./set_elementtype/) | सेट करता है कि विस्तारित एट्रिब्यूट टास्क, रिसोर्स या असाइनमेंट से जुड़ा है। |
| [set_FieldId](./set_fieldid/) | सेट करता है जो कस्टम फ़ील्ड के प्रोजेक्ट आईडी से मेल खाता है। FieldId प्रॉपर्टी निर्दिष्ट करने के लिए Aspose::Tasks::ExtendedAttributeTask क्लास के एक स्थिरांक की स्ट्रिंग प्रतिनिधित्व का उपयोग करें। |
| [set_Formula](./set_formula/) | Microsoft Project द्वारा कस्टम टास्क फ़ील्ड को भरने के लिए उपयोग की जाने वाली फ़ॉर्मूला सेट करता है। |
| [set_GraphicalIndicator](./set_graphicalindicator/) | विस्तारित एट्रिब्यूट से जुड़ी ग्राफिकल इंडिकेटर्स जानकारी सेट करता है। MPP फ़ॉर्मेट के लिए लागू। |
| [set_Guid](./set_guid/) | कस्टम फ़ील्ड का Guid सेट करता है। |
| [set_MaxMultiValues](./set_maxmultivalues/) | पिक लिस्ट में आप जितने अधिकतम मान सेट कर सकते हैं, उसे सेट करता है। |
| [set_PhoneticsAlias](./set_phoneticsalias/) | कस्टम फ़ील्ड के उपनाम की ध्वन्यात्मक उच्चारण सेट करता है। |
| [set_RestrictValues](./set_restrictvalues/) | एक मान सेट करता है जो दर्शाता है कि कस्टम फ़ील्ड मान ValueList में मानों तक सीमित हैं या नहीं। |
| [set_RollupType](./set_rolluptype/) | रोलअप्स की गणना का तरीका सेट करता है। |
| [set_SecondaryGuid](./set_secondaryguid/) | विस्तारित एट्रिब्यूट का द्वितीयक guid सेट करता है। |
| [set_SecondaryPid](./set_secondarypid/) | कस्टम फ़ील्ड का द्वितीयक PID सेट करता है। |
| [set_SummaryRowsCalculationType](./set_summaryrowscalculationtype/) | समरी रो के लिए कस्टम एट्रिब्यूट के मान की गणना प्रकार सेट करता है। |
| [set_UserDef](./set_userdef/) | एक मान सेट करता है जो दर्शाता है कि कस्टम फ़ील्ड उपयोगकर्ता द्वारा परिभाषित है या नहीं। |
| [set_ValuelistSortOrder](./set_valuelistsortorder/) | वैल्यू लिस्ट्स को सॉर्ट करने का तरीका सेट करता है। मान हैं: 0=अवरोही, 1=आरोही। |

