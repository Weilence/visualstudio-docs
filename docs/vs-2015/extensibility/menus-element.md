---
title: "Menus Element | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "VSCT XML schema elements, Menus"
  - "Menus element (VSCT XML schema)"
ms.assetid: d825a99b-e05c-4dd9-8933-a180216d667a
caps.latest.revision: 11
ms.author: "gregvanl"
manager: "ghogen"
---
# Menus Element
[!INCLUDE[vs2017banner](../includes/vs2017banner.md)]

The latest version of this topic can be found at [Menus Element](https://docs.microsoft.com/visualstudio/extensibility/menus-element).  
  
Defines all the menus and toolbars that a VSPackage implements.  
  
## Syntax  
  
```  
<Menus>  
  <Menu>... </Menu>  
  <Menu>... </Menu>  
</Menus>  
```  
  
## Attributes and Elements  
 The following sections describe attributes, child elements, and parent elements.  
  
### Attributes  
  
|Attribute|Description|  
|---------------|-----------------|  
|Condition|Optional. See [Conditional Attributes](../extensibility/vsct-xml-schema-conditional-attributes.md).|  
  
### Child Elements  
  
|Element|Description|  
|-------------|-----------------|  
|[Menus Element](../extensibility/menus-element.md)|Defines all the menus and toolbars that a VSPackage implements.|  
|[Menu Element](../extensibility/menu-element.md)|Represents a single menu or toolbar.|  
  
### Parent Elements  
  
|Element|Description|  
|-------------|-----------------|  
|[Commands Element](../extensibility/commands-element.md)|Represents the collection of commands in the VSPackage.|  
  
## Example  
  
```  
<Commands package="guidMyPackage">  
    <Menus>  
      <Menu Condition="'%(DEBUG)' != 'true'"   
        guid="cmdSetGuidMyProductCommands" id="menuIDMainMenu"   
        priority="0x0000" type="Menu">  
        <Annotation>  
          <Documentation>this is an annotation</Documentation>  
          <AppInfo>  
            <CustomData>  
              <CustomSubElement>Some data</CustomSubElement>  
            </CustomData>  
          </AppInfo>  
        </Annotation>  
        <CommandFlag>AlwaysCreate</CommandFlag>  
        <Strings>  
          <ButtonText>MainMenu</ButtonText>  
        </Strings>  
      </Menu>  
  </Menus>  
<Commands>  
```  
  
## See Also  
 [How VSPackages Add User Interface Elements](../extensibility/internals/how-vspackages-add-user-interface-elements.md)   
 [Commands, Menus, and Toolbars](../extensibility/internals/commands-menus-and-toolbars.md)

