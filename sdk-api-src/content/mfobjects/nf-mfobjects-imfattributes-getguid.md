---
UID: NF:mfobjects.IMFAttributes.GetGUID
title: IMFAttributes::GetGUID (mfobjects.h)
description: Retrieves a GUID value associated with a key.
helpviewer_keywords: ["6ded35e1-2d1c-4e68-ad0f-2bd5ba469853","GetGUID","GetGUID method [Media Foundation]","GetGUID method [Media Foundation]","IMFAttributes interface","IMFAttributes interface [Media Foundation]","GetGUID method","IMFAttributes.GetGUID","IMFAttributes::GetGUID","mf.imfattributes_getguid","mfobjects/IMFAttributes::GetGUID"]
old-location: mf\imfattributes_getguid.htm
tech.root: medfound
ms.assetid: 6ded35e1-2d1c-4e68-ad0f-2bd5ba469853
ms.date: 12/05/2018
ms.keywords: 6ded35e1-2d1c-4e68-ad0f-2bd5ba469853, GetGUID, GetGUID method [Media Foundation], GetGUID method [Media Foundation],IMFAttributes interface, IMFAttributes interface [Media Foundation],GetGUID method, IMFAttributes.GetGUID, IMFAttributes::GetGUID, mf.imfattributes_getguid, mfobjects/IMFAttributes::GetGUID
f1_keywords:
- mfobjects/IMFAttributes.GetGUID
dev_langs:
- c++
req.header: mfobjects.h
req.include-header: Mfidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Mfuuid.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- mfuuid.lib
- mfuuid.dll
api_name:
- IMFAttributes.GetGUID
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IMFAttributes::GetGUID


## -description



Retrieves a GUID value associated with a key.




## -parameters




### -param guidKey [in]

GUID that identifies which value to retrieve. The attribute type must be <b>MF_ATTRIBUTE_GUID</b>.


### -param pguidValue [out]

Receives a GUID value. If the key is found and the data type is GUID, the method copies the value into this parameter. Otherwise, the original value of this parameter is not changed.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MF_E_ATTRIBUTENOTFOUND</b></dt>
</dl>
</td>
<td width="60%">
The specified key was not found.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MF_E_INVALIDTYPE</b></dt>
</dl>
</td>
<td width="60%">
The attribute value is not a GUID.

</td>
</tr>
</table>
 




## -remarks



This interface is available on the following platforms if the Windows Media Format 11 SDK redistributable components are installed:

<ul>
<li>Windows XP with Service Pack 2 (SP2) and later.</li>
<li>Windows XP Media Center Edition 2005 with KB900325 (Windows XP Media Center Edition 2005) and KB925766 (October 2006 Update Rollup for Windows XP Media Center Edition) installed.</li>
</ul>



## -see-also




<a href="https://docs.microsoft.com/windows/desktop/medfound/attributes-and-properties">Attributes and Properties</a>



<a href="https://docs.microsoft.com/windows/desktop/api/mfobjects/nn-mfobjects-imfattributes">IMFAttributes</a>



<a href="https://docs.microsoft.com/windows/desktop/api/mfobjects/ne-mfobjects-mf_attribute_type">MF_ATTRIBUTE_TYPE</a>
 

 

