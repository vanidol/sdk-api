---
UID: NN:comsvcs.IComTransactionEvents
title: IComTransactionEvents (comsvcs.h)
description: Notifies the subscriber if the Microsoft Distributed Transaction Coordinator (DTC) transaction starts, commits, or aborts.
helpviewer_keywords: ["IComTransactionEvents","IComTransactionEvents interface [COM+]","IComTransactionEvents interface [COM+]","described","_dtc_IComTransactionEvents","comsvcs/IComTransactionEvents","cos.icomtransactionevents"]
old-location: cos\icomtransactionevents.htm
tech.root: cossdk
ms.assetid: f28a0ef5-1c9a-4fdc-bb10-2c381f22f5e3
ms.date: 12/05/2018
ms.keywords: IComTransactionEvents, IComTransactionEvents interface [COM+], IComTransactionEvents interface [COM+],described, _dtc_IComTransactionEvents, comsvcs/IComTransactionEvents, cos.icomtransactionevents
f1_keywords:
- comsvcs/IComTransactionEvents
dev_langs:
- c++
req.header: comsvcs.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- ComSvcs.h
api_name:
- IComTransactionEvents
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IComTransactionEvents interface


## -description


Notifies the subscriber if the Microsoft Distributed Transaction Coordinator (DTC) transaction starts, commits, or aborts. The subscriber is also notified when the resource manager retrieves prepare information from the transaction manager. The events are published to the subscriber using the <a href="https://docs.microsoft.com/windows/desktop/cossdk/com--events">COM+ Events</a> service, a loosely coupled events system that stores event information from different publishers in an event store in the COM+ catalog.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IComTransactionEvents</b> interface inherits from the <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nn-unknwn-iunknown">IUnknown</a> interface. <b>IComTransactionEvents</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IComTransactionEvents</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/comsvcs/nf-comsvcs-icomtransactionevents-ontransactionabort">OnTransactionAbort</a>
</td>
<td align="left" width="63%">
Generated when a transaction aborts.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/comsvcs/nf-comsvcs-icomtransactionevents-ontransactioncommit">OnTransactionCommit</a>
</td>
<td align="left" width="63%">
Generated when a transaction commits.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/comsvcs/nf-comsvcs-icomtransactionevents-ontransactionprepare">OnTransactionPrepare</a>
</td>
<td align="left" width="63%">
Generated when the prepare phase of the two-phase commit protocol of the transaction is completed.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/comsvcs/nf-comsvcs-icomtransactionevents-ontransactionstart">OnTransactionStart</a>
</td>
<td align="left" width="63%">
Generated when a Microsoft Distributed Transaction Coordinator (DTC) transaction starts.

</td>
</tr>
</table> 


## -see-also




<a href="https://docs.microsoft.com/windows/desktop/cossdk/com--events">COM+ Events</a>



<a href="https://docs.microsoft.com/windows/desktop/cossdk/com--instrumentation-concepts">COM+ Instrumentation</a>



<a href="https://docs.microsoft.com/windows/desktop/cossdk/com--transactions">COM+ Transactions</a>
 

 

