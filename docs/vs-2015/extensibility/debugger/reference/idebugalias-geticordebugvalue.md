---
title: "IDebugAlias::GetICorDebugValue | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "IDebugAlias::GetICorDebugValue"
helpviewer_keywords: 
  - "IDebugAlias::GetICorDebugValue method"
ms.assetid: b9eb39ee-84af-4ace-9cfe-236b3d48aff5
caps.latest.revision: 13
ms.author: "gregvanl"
manager: "ghogen"
---
# IDebugAlias::GetICorDebugValue
[!INCLUDE[vs2017banner](../../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDebugAlias::GetICorDebugValue](https://docs.microsoft.com/visualstudio/extensibility/debugger/reference/idebugalias-geticordebugvalue).  
  
Retrieves a managed code interface that represents the value associated with this alias.  
  
## Syntax  
  
```cpp  
HRESULT GetICorDebugValue(  
   IUnknown** ppUnk  
);  
```  
  
```csharp  
int GetICorDebugValue(  
   out object ppUnk  
);  
```  
  
#### Parameters  
 `ppUnk`  
 [out] `IUnknown` interface that represents the value associated with this alias. This interface can be queried for the `ICorDebugValue` interface.  
  
## Return Value  
 If successful, returns S_OK; otherwise, returns an error code.  
  
## Remarks  
 This method applies only to managed values (the `ICorDebugValue` is an interface available in the [!INCLUDE[dnprdnshort](../../../includes/dnprdnshort-md.md)] and is defined in the [!INCLUDE[dnprdnshort](../../../includes/dnprdnshort-md.md)] SDK in the cordebug.idl file).  
  
## See Also  
 [IDebugAlias](../../../extensibility/debugger/reference/idebugalias.md)

