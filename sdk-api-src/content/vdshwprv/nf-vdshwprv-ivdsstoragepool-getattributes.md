---
UID: NF:vdshwprv.IVdsStoragePool.GetAttributes
title: IVdsStoragePool::GetAttributes (vdshwprv.h)
description: Returns the attributes of a storage pool.
helpviewer_keywords: ["GetAttributes","GetAttributes method","GetAttributes method","IVdsStoragePool interface","IVdsStoragePool interface","GetAttributes method","IVdsStoragePool.GetAttributes","IVdsStoragePool::GetAttributes","base.ivdsstoragepool_getattributes","vds/IVdsStoragePool::GetAttributes","vdshwprv/IVdsStoragePool::GetAttributes"]
old-location: base\ivdsstoragepool_getattributes.htm
tech.root: VDS
ms.assetid: 44906c1f-ecb2-4701-9392-a9b5924e9d65
ms.date: 12/05/2018
ms.keywords: GetAttributes, GetAttributes method, GetAttributes method,IVdsStoragePool interface, IVdsStoragePool interface,GetAttributes method, IVdsStoragePool.GetAttributes, IVdsStoragePool::GetAttributes, base.ivdsstoragepool_getattributes, vds/IVdsStoragePool::GetAttributes, vdshwprv/IVdsStoragePool::GetAttributes
f1_keywords:
- vdshwprv/IVdsStoragePool.GetAttributes
dev_langs:
- c++
req.header: vdshwprv.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Uuid.lib
- Uuid.dll
api_name:
- IVdsStoragePool.GetAttributes
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IVdsStoragePool::GetAttributes


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://docs.microsoft.com/windows/desktop/VDS/virtual-disk-service-portal">Virtual Disk Service</a> COM interface is superseded by the <a href="https://docs.microsoft.com/previous-versions/windows/desktop/stormgmt/windows-storage-management-api-portal">Windows Storage Management API</a>.]

Returns the attributes of a <a href="https://docs.microsoft.com/windows/desktop/VDS/storage-pool-object">storage pool</a>.


## -parameters




### -param pStoragePoolAttributes [out]

The address of a caller-allocated <a href="https://docs.microsoft.com/windows/desktop/api/vdshwprv/ns-vdshwprv-vds_pool_attributes">VDS_POOL_ATTRIBUTES</a> structure that receives the storage pool attributes.


## -returns



This method can return standard HRESULT values, such as E_INVALIDARG or E_OUTOFMEMORY, and <a href="https://docs.microsoft.com/windows/desktop/VDS/virtual-disk-service-common-return-codes">VDS-specific return values</a>. It can also return converted <a href="https://docs.microsoft.com/windows/desktop/Debug/system-error-codes">system error codes</a>  using the <a href="https://docs.microsoft.com/windows/desktop/api/winerror/nf-winerror-hresult_from_win32">HRESULT_FROM_WIN32</a> macro. Errors can originate from VDS itself or from the underlying <a href="https://docs.microsoft.com/windows/desktop/VDS/about-vds">VDS provider</a> that is being used. Possible return values include the following.

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
The method completed successfully.

</td>
</tr>
</table>
 




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/vdshwprv/nn-vdshwprv-ivdsstoragepool">IVdsStoragePool</a>
 

 

