---
title: "IDebugExpressionContext2::GetName | Microsoft Docs"
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
  - "IDebugExpressionContext2::GetName"
helpviewer_keywords: 
  - "IDebugExpressionContext2::GetName"
ms.assetid: c2b70d22-17af-4986-a7e3-930910367216
caps.latest.revision: 11
ms.author: "gregvanl"
manager: "ghogen"
---
# IDebugExpressionContext2::GetName
[!INCLUDE[vs2017banner](../../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDebugExpressionContext2::GetName](https://docs.microsoft.com/visualstudio/extensibility/debugger/reference/idebugexpressioncontext2-getname).  
  
Retrieves the name of the evaluation context.  
  
## Syntax  
  
```cpp#  
HRESULT GetName(   
   BSTR* pbstrName  
);  
```  
  
```csharp  
int GetName(   
   out string pbstrName  
);  
```  
  
#### Parameters  
 `pbstrName`  
 [out] Returns the name of the evaluation context.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns an error code.  
  
## Remarks  
 The name is the description of this evaluation context. It is typically something that can be parsed by an expression evaluator that refers to this exact evaluation context. For example, in C++ the name is as follows:  
  
```  
"{ function-name, source-file-name, module-file-name }"  
```  
  
## See Also  
 [IDebugExpressionContext2](../../../extensibility/debugger/reference/idebugexpressioncontext2.md)

