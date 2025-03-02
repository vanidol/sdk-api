---
UID: NF:tapi3cc.ITAgent.get_User
title: ITAgent::get_User (tapi3cc.h)
description: The get_User method gets the agent user name, which is the same as the operating system user login or e-mail name.
helpviewer_keywords: ["ITAgent interface [TAPI 2.2]","get_User method","ITAgent.get_User","ITAgent::get_User","_tapi3_itagent_get_user","get_User","get_User method [TAPI 2.2]","get_User method [TAPI 2.2]","ITAgent interface","tapi3.itagent_get_user","tapi3cc/ITAgent::get_User"]
old-location: tapi3\itagent_get_user.htm
tech.root: Tapi
ms.assetid: 6949fdb0-5841-4473-bb50-2ea598a71576
ms.date: 12/05/2018
ms.keywords: ITAgent interface [TAPI 2.2],get_User method, ITAgent.get_User, ITAgent::get_User, _tapi3_itagent_get_user, get_User, get_User method [TAPI 2.2], get_User method [TAPI 2.2],ITAgent interface, tapi3.itagent_get_user, tapi3cc/ITAgent::get_User
f1_keywords:
- tapi3cc/ITAgent.get_User
dev_langs:
- c++
req.header: tapi3cc.h
req.include-header: Tapi3.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Tapi3.dll
api_name:
- ITAgent.get_User
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ITAgent::get_User


## -description


The 
<b>get_User</b> method gets the agent user name, which is the same as the operating system user login or e-mail name.


## -parameters




### -param ppUser [out]

Pointer to <b>BSTR</b> containing user name.


## -returns



This method can return one of these values.

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
Method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>ppUser</i> parameter is not a valid pointer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory exists to perform the operation.

</td>
</tr>
</table>
 




## -remarks



The application must free the memory allocated for the <i>ppUser</i> parameter through 
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/oleauto/nf-oleauto-sysfreestring">SysFreeString</a> when the variable is no longer needed.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/tapi3/nn-tapi3-itagent">ITAgent</a>
 

 

