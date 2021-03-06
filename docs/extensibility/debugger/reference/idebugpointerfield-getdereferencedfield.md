---
title: "IDebugPointerField::GetDereferencedField | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.technology: 
  - "vs-ide-sdk"
ms.topic: "conceptual"
f1_keywords: 
  - "IDebugPointerField::GetDereferencedField"
helpviewer_keywords: 
  - "IDebugPointerField::GetDereferencedField method"
ms.assetid: 8de988ab-cd79-4287-be72-3c900f2fe407
author: "gregvanl"
ms.author: "gregvanl"
manager: douge
ms.workload: 
  - "vssdk"
---
# IDebugPointerField::GetDereferencedField
This method returns the type of object to which this pointer object points.  
  
## Syntax  
  
```cpp  
HRESULT GetDereferencedField(  
   IDebugField** ppField  
);  
```  
  
```csharp  
int GetDereferencedField(  
   out IDebugField ppField  
);  
```  
  
#### Parameters  
 `ppField`  
 [out] Returns an [IDebugField](../../../extensibility/debugger/reference/idebugfield.md) describing the type of target object.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns an error code.  
  
## Remarks  
 If, for example, the [IDebugPointerField](../../../extensibility/debugger/reference/idebugpointerfield.md) object points to an integer, the [IDebugField](../../../extensibility/debugger/reference/idebugfield.md) type returned by this method describes that integer type.  
  
## See Also  
 [IDebugPointerField](../../../extensibility/debugger/reference/idebugpointerfield.md)   
 [IDebugField](../../../extensibility/debugger/reference/idebugfield.md)