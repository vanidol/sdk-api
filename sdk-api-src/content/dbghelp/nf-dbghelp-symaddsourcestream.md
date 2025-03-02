---
UID: NF:dbghelp.SymAddSourceStream
title: SymAddSourceStream function (dbghelp.h)
description: Adds the stream to the specified module for use by the Source Server.
helpviewer_keywords: ["SymAddSourceStream","SymAddSourceStream function","SymAddSourceStreamW","base.symaddsourcestream","dbghelp/SymAddSourceStream","dbghelp/SymAddSourceStreamW"]
old-location: base\symaddsourcestream.htm
tech.root: Debug
ms.assetid: 1f85a5d3-70dc-430f-9a54-7cc08484ca93
ms.date: 12/05/2018
ms.keywords: SymAddSourceStream, SymAddSourceStream function, SymAddSourceStreamW, base.symaddsourcestream, dbghelp/SymAddSourceStream, dbghelp/SymAddSourceStreamW
f1_keywords:
- dbghelp/SymAddSourceStream
dev_langs:
- c++
req.header: dbghelp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: SymAddSourceStreamW (Unicode) and SymAddSourceStream (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Dbghelp.lib
req.dll: Dbghelp.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- Dbghelp.dll
api_name:
- SymAddSourceStream
- SymAddSourceStream
- SymAddSourceStreamW
targetos: Windows
req.typenames: 
req.redist: DbgHelp.dll 6.8 or later
ms.custom: 19H1
---

# SymAddSourceStream function


## -description


Adds the stream to the specified module for use by the <a href="https://docs.microsoft.com/windows/desktop/Debug/source-server-and-source-indexing">Source Server</a>.


## -parameters




### -param hProcess [in]

A handle to a process. This handle must have been previously passed to the 
<a href="https://docs.microsoft.com/windows/desktop/api/dbghelp/nf-dbghelp-syminitialize">SymInitialize</a> function.


### -param Base [in]

The base address of the module.


### -param StreamFile [in, optional]

A null-terminated string that contains the absolute or relative path to a file that contains the source indexing stream. Can be <b>NULL</b> if <i>Buffer</i> is not <b>NULL</b>.


### -param Buffer [in, optional]

A buffer that contains the source indexing stream. Can be <b>NULL</b> if <i>StreamFile</i> is not <b>NULL</b>.


### -param Size [in]

Size, in bytes, of the <i>Buffer</i> buffer.


## -returns



If the function succeeds, the return value is <b>TRUE</b>.

If the function fails, the return value is <b>FALSE</b>. To retrieve extended error information, call 
<a href="https://docs.microsoft.com/windows/desktop/api/errhandlingapi/nf-errhandlingapi-getlasterror">GetLastError</a>.




## -remarks



<b>SymAddSourceStream</b> adds a stream of data formatted for use by the <a href="https://docs.microsoft.com/windows/desktop/Debug/source-server-and-source-indexing">source Server</a> to a designated module.  The caller can pass the stream either as a buffer in the <i>Buffer</i> parameter or a file in the <i>StreamFile</i> parameter.  If both parameters are filled, then the function uses the   <i>Buffer</i> parameter.  If both parameters are <b>NULL</b>, then the function returns <b>FALSE</b> and the <a href="https://docs.microsoft.com/windows/desktop/Debug/last-error-code">last-error code</a> is set to <b>ERROR_INVALID_PARAMETER</b>.

It is important to note that <b>SymAddSourceStream</b> does not add the stream to any corresponding PDB in order to persist the data.  This function is used by those programmatically implementing their own debuggers in scenarios in which a PDB is not available.



