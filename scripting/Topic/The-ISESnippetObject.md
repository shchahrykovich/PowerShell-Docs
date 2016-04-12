---
title: The ISESnippetObject
ms.custom: na
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 98bc8113-c3cd-4201-bdb9-9d9bdb7e266c
---
# The ISESnippetObject
  An **ISESnippet** object is an instance of the Microsoft.PowerShell.Host.ISE.ISESnippet class. The members of the **$psISE.CurrentPowerShellTab.Snippets** collection are all examples of **ISESnippet** objects. The easiest way to create a snippet is to use the [New\-IseSnippet&#91;PSITPro5\_ISE&#93;](assetId:///0a6339a3-2683-4a8e-8929-90ad9a95c3e0) cmdlet.

## Properties

###  <a name="DisplayName"></a> Author
 [!INCLUDE[support_ise_3up](../Token/support_ise_3up_md.md)]

 The read\-only property that gets the name of the author of the snippet.

```
# Get the author of the first snippet item
$psISE.CurrentPowerShellTab.Snippets.Item(0).Author

```

###  <a name="Action"></a> CodeFragment
 [!INCLUDE[support_ise_3up](../Token/support_ise_3up_md.md)]

 The read\-only property that gets the code fragment to be inserted into the editor.

```
# Get the code fragment associated with the first snippet item.
$psISE.CurrentPowerShellTab.Snippets.Item(0).CodeFragment

```

###  <a name="Shortcut"></a> Shortcut
 [!INCLUDE[support_ise_3up](../Token/support_ise_3up_md.md)]

 The read\-only property that gets the Windows keyboard shortcut for the menu item.

```
# Get the shortcut for the first submenu item.
$psISE.CurrentPowerShellTab.AddOnsMenu.SubMenus.Clear()
$psISE.CurrentPowerShellTab.AddOnsMenu.SubMenus.Add("_Process",{get-process},"Alt+P")
$psISE.CurrentPowerShellTab.AddOnsMenu.Submenus[0].Shortcut
```

## See Also
 [The ISESnippetCollection Object](../Topic/The-ISESnippetCollection-Object.md) 
 [The Windows PowerShell ISE Scripting Object Model](../Topic/The-Windows-PowerShell-ISE-Scripting-Object-Model.md) 
 [Windows PowerShell ISE Object Model Reference](../Topic/Windows-PowerShell-ISE-Object-Model-Reference.md) 
 [The ISE Object Model Hierarchy](../Topic/The-ISE-Object-Model-Hierarchy.md)

  