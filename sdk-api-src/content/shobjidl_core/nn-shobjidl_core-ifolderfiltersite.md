---
UID: NN:shobjidl_core.IFolderFilterSite
title: IFolderFilterSite (shobjidl_core.h)
description: Exported by a host to allow clients to specify how to filter a Shell folder enumeration.
helpviewer_keywords: ["IFolderFilterSite","IFolderFilterSite interface [Windows Shell]","IFolderFilterSite interface [Windows Shell]","described","_shell_IFolderFilterSite","shell.IFolderFilterSite","shobjidl_core/IFolderFilterSite"]
old-location: shell\IFolderFilterSite.htm
tech.root: shell
ms.assetid: 8b6fe1a3-9977-42a8-af95-da0fc6809b1b
ms.date: 12/05/2018
ms.keywords: IFolderFilterSite, IFolderFilterSite interface [Windows Shell], IFolderFilterSite interface [Windows Shell],described, _shell_IFolderFilterSite, shell.IFolderFilterSite, shobjidl_core/IFolderFilterSite
f1_keywords:
- shobjidl_core/IFolderFilterSite
dev_langs:
- c++
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shobjidl.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Shell32.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Shell32.dll
api_name:
- IFolderFilterSite
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IFolderFilterSite interface


## -description


Exported by a host to allow clients to specify how to filter a Shell folder enumeration.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IFolderFilterSite</b> interface inherits from the <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nn-unknwn-iunknown">IUnknown</a> interface. <b>IFolderFilterSite</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IFolderFilterSite</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/shobjidl_core/nf-shobjidl_core-ifolderfiltersite-setfilter">SetFilter</a>
</td>
<td align="left" width="63%">
Exposed by a host to allow clients to pass the host their <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nn-unknwn-iunknown">IUnknown</a> interface pointers.

</td>
</tr>
</table> 


## -remarks



The most common use of this interface is when your application calls <a href="https://docs.microsoft.com/windows/desktop/api/shlobj_core/nf-shlobj_core-shbrowseforfoldera">SHBrowseForFolder</a>. When you call this function, you become a client of the folder browser object. That object communicates with you by sending messages to a callback function, <a href="https://docs.microsoft.com/previous-versions/windows/desktop/legacy/bb762598(v=vs.85)">BrowseCallbackProc</a>. The BFFM_IUNKNOWN message contains a pointer to the folder browser's <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nn-unknwn-iunknown">IUnknown</a> interface. To filter folder enumeration:



<ol>
<li>Use the <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nn-unknwn-iunknown">IUnknown</a> pointer to call the folder browser's <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nf-unknwn-iunknown-queryinterface(q)">QueryInterface</a> method, and request a pointer to the <b>IFolderFilterSite</b> interface.</li>
<li>Call <a href="https://docs.microsoft.com/windows/desktop/api/shobjidl_core/nf-shobjidl_core-ifolderfiltersite-setfilter">IFolderFilterSite::SetFilter</a>, and pass the folder browser a pointer to your <a href="https://docs.microsoft.com/windows/desktop/api/shobjidl_core/nn-shobjidl_core-ifolderfilter">IFolderFilter</a> (IUnknown or IFilterFolder?) interface.</li>
<li>The folder browser will then query the two methods of the <b>IFolderFilterSite</b> interface to determine how to filter the enumeration.</li>
</ol>


