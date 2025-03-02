---
UID: NN:d3d12.ID3D12DeviceRemovedExtendedData
title: ID3D12DeviceRemovedExtendedData interface
description: Provides runtime access to Device Removed Extended Data (DRED) data.
helpviewer_keywords: ["ID3D12DeviceRemovedExtendedData","ID3D12DeviceRemovedExtendedData interface","ID3D12DeviceRemovedExtendedData interface","described","d3d12/ID3D12DeviceRemovedExtendedData","direct3d12.id3d12deviceremovedextendeddata"]
tech.root: direct3d12
ms.date: 02/08/2019
ms.keywords: ID3D12DeviceRemovedExtendedData, ID3D12DeviceRemovedExtendedData interface, ID3D12DeviceRemovedExtendedData interface,described, d3d12/ID3D12DeviceRemovedExtendedData, direct3d12.id3d12deviceremovedextendeddata
f1_keywords:
- d3d12/ID3D12DeviceRemovedExtendedData
dev_langs:
- c++
req.header: d3d12.h
req.include-header: 
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
req.lib: D3D12.lib
req.dll: D3D12.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- D3D12.dll
api_name:
- ID3D12DeviceRemovedExtendedData
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ID3D12DeviceRemovedExtendedData interface

## -description

Provides runtime access to Device Removed Extended Data (DRED) data. To retrieve the **ID3D12DeviceRemovedExtendedData** interface, call [QueryInterface](/windows/desktop/api/unknwn/nf-unknwn-iunknown-queryinterface(refiid_void)) on an [ID3D12Device](nn-d3d12-id3d12device.md) (or derived) interface, passing the interface identifier (IID) of **ID3D12DeviceRemovedExtendedData**.

## Inheritance

The **ID3D12DeviceRemovedExtendedData** interface inherits from the [IUnknown](/windows/desktop/api/unknwn/nn-unknwn-iunknown) interface.

## -members

The **ID3D12DeviceRemovedExtendedData** interface has these methods.

|Method|Description|
|-|-|
|[GetAutoBreadcrumbsOutput](nf-d3d12-id3d12deviceremovedextendeddata-getautobreadcrumbsoutput.md)|Retrieves the Device Removed Extended Data (DRED) auto-breadcrumbs output.|
|[GetPageFaultAllocationOutput](nf-d3d12-id3d12deviceremovedextendeddata-getpagefaultallocationoutput.md)|Retrieves the Device Removed Extended Data (DRED) page fault data.|

## -remarks

## -see-also

* [Core interfaces](/windows/desktop/direct3d12/direct3d-12-interfaces)
* [Use DRED to diagnose GPU faults](/windows/desktop/direct3d12/use-dred)
