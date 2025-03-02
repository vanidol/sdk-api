---
UID: NF:mfcaptureengine.IMFCapturePhotoSink.SetOutputFileName
title: IMFCapturePhotoSink::SetOutputFileName (mfcaptureengine.h)
description: Specifies the name of the output file for the still image.
helpviewer_keywords: ["IMFCapturePhotoSink interface [Media Foundation]","SetOutputFileName method","IMFCapturePhotoSink.SetOutputFileName","IMFCapturePhotoSink::SetOutputFileName","SetOutputFileName","SetOutputFileName method [Media Foundation]","SetOutputFileName method [Media Foundation]","IMFCapturePhotoSink interface","mf.imfcapturephotosink_setoutputfilename","mfcaptureengine/IMFCapturePhotoSink::SetOutputFileName"]
old-location: mf\imfcapturephotosink_setoutputfilename.htm
tech.root: medfound
ms.assetid: CAA9F7CF-A92F-4039-BEA5-07A730E82EE4
ms.date: 12/05/2018
ms.keywords: IMFCapturePhotoSink interface [Media Foundation],SetOutputFileName method, IMFCapturePhotoSink.SetOutputFileName, IMFCapturePhotoSink::SetOutputFileName, SetOutputFileName, SetOutputFileName method [Media Foundation], SetOutputFileName method [Media Foundation],IMFCapturePhotoSink interface, mf.imfcapturephotosink_setoutputfilename, mfcaptureengine/IMFCapturePhotoSink::SetOutputFileName
f1_keywords:
- mfcaptureengine/IMFCapturePhotoSink.SetOutputFileName
dev_langs:
- c++
req.header: mfcaptureengine.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
- mfcaptureengine.h
api_name:
- IMFCapturePhotoSink.SetOutputFileName
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IMFCapturePhotoSink::SetOutputFileName


## -description


Specifies the name of the output file for the still image.


## -parameters




### -param fileName [in]

A null-terminated string that contains the URL of the output file. 


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Calling this method overrides any previous call to <a href="https://docs.microsoft.com/windows/desktop/api/mfcaptureengine/nf-mfcaptureengine-imfcapturephotosink-setoutputbytestream">IMFCapturePhotoSink::SetOutputByteStream</a> or <a href="https://docs.microsoft.com/windows/desktop/api/mfcaptureengine/nf-mfcaptureengine-imfcapturephotosink-setsamplecallback">IMFCapturePhotoSink::SetSampleCallback</a>.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/mfcaptureengine/nn-mfcaptureengine-imfcapturephotosink">IMFCapturePhotoSink</a>
 

 

