---
title: The ISEAddOnTool Object
ms.custom: na
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: ce84d8bc-07ba-41f6-bdde-d6f3fddcd1e3
---
# The ISEAddOnTool Object
  An **ISEAddonTool** object represents an installed add\-on tool that provides additional functionality to[!INCLUDE[ise_2](../Token/ise_2_md.md)]. An example is the **Commands** tool that you can display by clicking **View**, then **Show Command Add\-on**. This tool is then accessible to you by manipulating the various available **ISEAddOnTool** objects.

 Each add\-on tool can be associated with either the vertical pane or the horizontal pane. The vertical pane is docked to the right edge of [!INCLUDE[ise_2](../Token/ise_2_md.md)]. The horizontal pane is docked to the bottom edge.

 Each PowerShell tab in [!INCLUDE[ise_2](../Token/ise_2_md.md)] can have its own set of add\-on tools installed. See [$psISE.CurrentPowerShellTab.HorizontalAddOnTools](../Topic/The-ISEAddOnToolCollection-Object.md) and [$psISE.CurrentPowerShellTab.VerticalAddOnTools](../Topic/The-ISEAddOnToolCollection-Object.md) to access the collection of tools available to the currently selected tab or the same properties on any of the **PowerShellTab** objects in the [$psISE.PowerShellTabs](../Topic/The-PowerShellTabCollection-Object.md) collection object.

## Methods
 There are no [!INCLUDE[ise_2](../Token/ise_2_md.md)]\-specific methods available for objects of this class.

## Properties

###  <a name="Control"></a> Control
 [!INCLUDE[support_ise_3up](../Token/support_ise_3up_md.md)]

 The **Control** property provides read access to many of the details of the Commands add\-on tool.

```
# View the properties of the Commands add-on tool.
# (assumes that it is visible in the vertical pane)
$psISE.CurrentVisibleVerticalTool.Control
HostObject                  : Microsoft.PowerShell.Host.ISE.ObjectModelRoot
Content                     : 
HasContent                  : 
ContentTemplate             : 
ContentTemplateSelector     : 
ContentStringFormat         : 
BorderBrush                 : 
BorderThickness             : 
Background                  : 
Foreground                  : 
FontFamily                  : 
FontSize                    : 
FontStretch                 : 
FontStyle                   : 
FontWeight                  : 
HorizontalContentAlignment  : 
VerticalContentAlignment    : 
TabIndex                    : 
IsTabStop                   : 
Padding                     : 
Template                    : System.Windows.Controls.ControlTemplate
Style                       : 
OverridesDefaultStyle       : 
UseLayoutRounding           : 
Triggers                    : {}
TemplatedParent             : 
Resources                   : {System.Windows.Controls.TabItem}
DataContext                 : 
BindingGroup                : 
Language                    : 
Name                        : 
Tag                         : 
InputScope                  : 
ActualWidth                 : 370.75
ActualHeight                : 676.559097412109
LayoutTransform             : 
Width                       : 
MinWidth                    : 
MaxWidth                    : 
Height                      : 
MinHeight                   : 
MaxHeight                   : 
FlowDirection               : LeftToRight
Margin                      : 
HorizontalAlignment         : 
VerticalAlignment           : 
FocusVisualStyle            : 
Cursor                      : 
ForceCursor                 : 
IsInitialized               : True
IsLoaded                    : 
ToolTip                     : 
ContextMenu                 : 
Parent                      : 
HasAnimatedProperties       : 
InputBindings               : 
CommandBindings             : 
AllowDrop                   : 
DesiredSize                 : 227.66,676.559097412109
IsMeasureValid              : True
IsArrangeValid              : True
RenderSize                  : 370.75,676.559097412109
RenderTransform             : 
RenderTransformOrigin       : 
IsMouseDirectlyOver         : False
IsMouseOver                 : False
IsStylusOver                : False
IsKeyboardFocusWithin       : False
IsMouseCaptured             : 
IsMouseCaptureWithin        : False
IsStylusDirectlyOver        : False
IsStylusCaptured            : 
IsStylusCaptureWithin       : False
IsKeyboardFocused           : False
IsInputMethodEnabled        : 
Opacity                     : 
OpacityMask                 : 
BitmapEffect                : 
Effect                      : 
BitmapEffectInput           : 
CacheMode                   : 
Uid                         : 
Visibility                  : Visible
ClipToBounds                : False
Clip                        : 
SnapsToDevicePixels         : False
IsFocused                   : 
IsEnabled                   : 
IsHitTestVisible            : 
IsVisible                   : True
Focusable                   : 
PersistId                   : 1
IsManipulationEnabled       : 
AreAnyTouchesOver           : False
AreAnyTouchesDirectlyOver   : 
AreAnyTouchesCapturedWithin : False
AreAnyTouchesCaptured       : 
TouchesCaptured             : {}
TouchesCapturedWithin       : {}
TouchesOver                 : {}
TouchesDirectlyOver         : {}
DependencyObjectType        : System.Windows.DependencyObjectType
IsSealed                    : False
Dispatcher                  : System.Windows.Threading.Dispatcher

```

###  <a name="IsVisible"></a> IsVisible
 [!INCLUDE[support_ise_3up](../Token/support_ise_3up_md.md)]

 The Boolean property that indicates whether the add\-on tool is currently visible in its assigned pane. If it is visible, you can set the **IsVisible** property to **$false** to hide the tool, or set the **IsVisible** property to **$true** to make an add\-on tool visible on its PowerShell tab. Note that after an add\-on tool is hidden, it is no longer accessible through the **CurrentVisibleHorizontalTool** or **CurrentVisibleVerticalTool** objects, and therefore cannot be made visible by using this property on that object.

```
# Hide the current tool in the vertical tool pane
$psISE.CurrentVisibleVerticalTool.IsVisible = $false
# Show the first tool on the currently selected PowerShell tab
$psISE.CurrentPowerShellTab.VerticalAddOnTools[0].IsVisible=$true

```

###  <a name="Commandpane"></a> Name
 [!INCLUDE[support_ise_3up](../Token/support_ise_3up_md.md)]

 The read\-only property that gets the name of the add\-on tool.

```
# Gets the name of the visible vertical pane add-on tool.
$psISE.CurrentVisibleVerticalTool.name
Commands

```

## See Also
 [The ISEAddOnToolCollection Object](../Topic/The-ISEAddOnToolCollection-Object.md) 
 [The Windows PowerShell ISE Scripting Object Model](../Topic/The-Windows-PowerShell-ISE-Scripting-Object-Model.md) 
 [Windows PowerShell ISE Object Model Reference](../Topic/Windows-PowerShell-ISE-Object-Model-Reference.md) 
 [The ISE Object Model Hierarchy](../Topic/The-ISE-Object-Model-Hierarchy.md)

  