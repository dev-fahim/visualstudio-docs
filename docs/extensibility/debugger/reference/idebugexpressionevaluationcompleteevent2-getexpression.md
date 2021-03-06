---
title: "IDebugExpressionEvaluationCompleteEvent2::GetExpression | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.technology: 
  - "vs-ide-sdk"
ms.topic: "conceptual"
f1_keywords: 
  - "IDebugExpressionEvaluationCompleteEvent2::GetExpression"
helpviewer_keywords: 
  - "IDebugExpressionEvaluationCompleteEvent2::GetExpression"
ms.assetid: faf6b2dd-2afd-4852-b21c-7e8d3130e141
author: "gregvanl"
ms.author: "gregvanl"
manager: douge
ms.workload: 
  - "vssdk"
---
# IDebugExpressionEvaluationCompleteEvent2::GetExpression
Gets the original expression.  
  
## Syntax  
  
```cpp  
HRESULT GetExpression(   
   IDebugExpression2** ppExpr  
);  
```  
  
```csharp  
int GetExpression(   
   out IDebugExpression2 ppExpr  
);  
```  
  
#### Parameters  
 `ppExpr`  
 [out] Returns an [IDebugExpression2](../../../extensibility/debugger/reference/idebugexpression2.md) object that represents the expression that was parsed.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns an error code.  
  
## Remarks  
 This method returns the object that was created in a call to the [ParseText](../../../extensibility/debugger/reference/idebugexpressioncontext2-parsetext.md) method.  
  
## See Also  
 [IDebugExpressionEvaluationCompleteEvent2](../../../extensibility/debugger/reference/idebugexpressionevaluationcompleteevent2.md)   
 [IDebugExpression2](../../../extensibility/debugger/reference/idebugexpression2.md)   
 [ParseText](../../../extensibility/debugger/reference/idebugexpressioncontext2-parsetext.md)