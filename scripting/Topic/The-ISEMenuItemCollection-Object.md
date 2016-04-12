---
title: The ISEMenuItemCollection Object
ms.custom: na
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 0c0f5484-3320-408e-8534-5bd1c8e48512
---
# The ISEMenuItemCollection Object
  An **ISEMenuItemCollection** object is a collection of **ISEMenuItem** objects. It is an instance of the Microsoft.PowerShell.Host.ISE.ISEMenuItemCollection class. An example is the **$psISE.CurrentPowerShellTab.AddOnsMenu.Submenus** object that is used to customize the **Add\-On** menu in [!INCLUDE[ise_1](../Token/ise_1_md.md)].

## Method

### Add\(string DisplayName, System.Management.Automation.ScriptBlock Action, System.Windows.Input.KeyGesture Shortcut \)
 [!INCLUDE[support_ise_2up](../Token/support_ise_2up_md.md)]

 Adds a menu item to the collection.

 **DisplayName**
 The display name of the menu to be added.

 **Action**
 The **System.Management.Automation.ScriptBlock** object that specifies the action that is associated with this menu item.

 **Shortcut**
 The keyboard shortcut for the action.

 **Returns**
 The ISEMenuItem object that was just added.

```
# Create an Add-ons menu with an fast access key and a shortcut.
# Note the use of "_"  as opposed to the "&" for mapping to the fast access key letter for the menu item.
$menuAdded = $psISE.CurrentPowerShellTab.AddOnsMenu.SubMenus.Add("_Process",{get-process},"Alt+P")
```

### Clear\(\)
 [!INCLUDE[support_ise_2up](../Token/support_ise_2up_md.md)]

 Removes all submenus from the menu item.

```
# Remove all custom submenu items from the AddOns menu
$psISE.CurrentPowerShellTab.AddOnsMenu.Submenus.Clear()

```

## See Also
 [The ISEMenuItem Object](../Topic/The-ISEMenuItem-Object.md) 
 [The Windows PowerShell ISE Scripting Object Model](../Topic/The-Windows-PowerShell-ISE-Scripting-Object-Model.md) 
 [Windows PowerShell ISE Object Model Reference](../Topic/Windows-PowerShell-ISE-Object-Model-Reference.md) 
 [The ISE Object Model Hierarchy](../Topic/The-ISE-Object-Model-Hierarchy.md)

  