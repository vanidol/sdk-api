---
UID: NF:control.IBasicVideo.put_SourceLeft
title: IBasicVideo::put_SourceLeft (control.h)
description: The put_SourceLeft method sets the x-coordinate of the source rectangle.
helpviewer_keywords: ["IBasicVideo interface [DirectShow]","put_SourceLeft method","IBasicVideo.put_SourceLeft","IBasicVideo::put_SourceLeft","IBasicVideoput_SourceLeft","control/IBasicVideo::put_SourceLeft","dshow.ibasicvideo_put_sourceleft","put_SourceLeft","put_SourceLeft method [DirectShow]","put_SourceLeft method [DirectShow]","IBasicVideo interface"]
old-location: dshow\ibasicvideo_put_sourceleft.htm
tech.root: DirectShow
ms.assetid: 0388d5fe-5434-41b9-b005-c0e4bf36bb27
ms.date: 12/05/2018
ms.keywords: IBasicVideo interface [DirectShow],put_SourceLeft method, IBasicVideo.put_SourceLeft, IBasicVideo::put_SourceLeft, IBasicVideoput_SourceLeft, control/IBasicVideo::put_SourceLeft, dshow.ibasicvideo_put_sourceleft, put_SourceLeft, put_SourceLeft method [DirectShow], put_SourceLeft method [DirectShow],IBasicVideo interface
f1_keywords:
- control/IBasicVideo.put_SourceLeft
dev_langs:
- c++
req.header: control.h
req.include-header: Dshow.h
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
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Strmiids.lib
- Strmiids.dll
api_name:
- IBasicVideo.put_SourceLeft
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IBasicVideo::put_SourceLeft


## -description



The <code>put_SourceLeft</code> method sets the x-coordinate of the source rectangle.




## -parameters




### -param SourceLeft [in]

Specifies the x-coordinate, in pixels.


## -returns



Returns an <b>HRESULT</b> value. Possible values include the following.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Invalid argument.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VFW_E_NOT_CONNECTED</b></dt>
</dl>
</td>
<td width="60%">
The video renderer's input pin is not connected.

</td>
</tr>
</table>
 




## -remarks



This method moves the entire source rectangle to the left or right. It does not change the width of the source rectangle. If the value of <i>SourceLeft</i> would place the right edge of the rectangle beyond the edge of the video frame, the method returns E_INVALIDARG. To crop the video, call <b>put_SourceWidth</b> to adjust the width, before calling <code>put_SourceLeft</code>. (Or call <b>SetSourcePosition</b> to set the entire source rectangle at once.)




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/DirectShow/error-and-success-codes">Error and Success Codes</a>



<a href="https://docs.microsoft.com/windows/desktop/api/control/nn-control-ibasicvideo">IBasicVideo Interface</a>
 

 

