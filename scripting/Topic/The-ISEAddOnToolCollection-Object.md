---
title: The ISEAddOnToolCollection Object
ms.custom: na
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 634eab89-0845-4016-974b-361b09bb8f7b
---
# The ISEAddOnToolCollection Object
  The **ISEAddOnToolCollection** object is a collection of **ISEAddOnTool** objects. An example is the **$psISE.CurrentPowerShellTab.VerticalAddOnTools** object.

## Methods

### Add\( Name, ControlType, \[IsVisible\] \)
 [!INCLUDE[support_ise_3up](../Token/support_ise_3up_md.md)]

 Adds a new add\-on tool to the collection. It returns the newly added add\-on tool. Before you run this command, you must install the add\-on tool on the local computer and load the assembly.

 **Name** – String
 Specifies the display name of the add\-on tool that is added to [!INCLUDE[ise_2](../Token/ise_2_md.md)].

 **ControlType** –Type
 Specifies the control that is added.

 **\[IsVisible\]** – optional Boolean
 If set to **$true**, the add\-on tool is immediately visible in the associated tool pane.

```
# Load a DLL with an add-on and then add it to the ISE
[reflection.assembly]::LoadFile("c:\test\ISESimpleSolution\ISESimpleSolution.dll")
$psISE.CurrentPowerShellTab.VerticalAddOnTools.Add("Solutions", [ISESimpleSolution.Solution], $true)

```

### Remove\( Item \)
 [!INCLUDE[support_ise_3up](../Token/support_ise_3up_md.md)]

 Removes the specified add\-on tool from the collection.

 **Item** – Microsoft.PowerShell.Host.ISE.ISEAddOnTool
 Specifies the object to be removed from [!INCLUDE[ise_2](../Token/ise_2_md.md)].

```
# Load a DLL with an add-on and then add it to the ISE
[reflection.assembly]::LoadFile("c:\test\ISESimpleSolution\ISESimpleSolution.dll")
$psISE.CurrentPowerShellTab.VerticalAddOnTools.Add("Solutions", [ISESimpleSolution.Solution], $true)

```

### SetSelectedPowerShellTab\( psTab \)
 [!INCLUDE[support_ise_3up](../Token/support_ise_3up_md.md)]

 Selects the PowerShell tab that the **psTab** parameter specifies.

 **psTab** – Microsoft.PowerShell.Host.ISE.PowerShellTab
 The PowerShell tab to select.

```

      $newTab = $psISE.PowerShellTabs.Add()
# Change the DisplayName of the new PowerShell tab. 
$newTab.DisplayName="Brand New Tab"

```

### Remove\( psTab \)
 [!INCLUDE[support_ise_3up](../Token/support_ise_3up_md.md)]

 Removes the PowerShell tab that the **psTab** parameter specifies.

 **psTab** – Microsoft.PowerShell.Host.ISE.PowerShellTab
 The PowerShell tab to remove.

```

$newTab = $psISE.PowerShellTabs.Add()
Change the DisplayName of the new PowerShell tab. 
$newTab.DisplayName="This tab will go away in 5 seconds" 
sleep 5 
$psISE.PowerShellTabs.Remove($newTab)
```

## See Also
 [The PowerShellTab Object](../Topic/The-PowerShellTab-Object.md) 
 [The Windows PowerShell ISE Scripting Object Model](../Topic/The-Windows-PowerShell-ISE-Scripting-Object-Model.md) 
 [Windows PowerShell ISE Object Model Reference](../Topic/Windows-PowerShell-ISE-Object-Model-Reference.md) 
 [The ISE Object Model Hierarchy](../Topic/The-ISE-Object-Model-Hierarchy.md)

  