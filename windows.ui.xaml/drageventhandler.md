---
-api-id: T:Windows.UI.Xaml.DragEventHandler
-api-type: winrt delegate
---
<!-- Delegate syntax.
public delegate void DragEventHandler(System.Object sender, Windows.UI.Xaml.DragEventArgs e)
-->
# Windows.UI.Xaml.DragEventHandler

## -description
Represents the method that will handle the [DragEnter](uielement_dragenter.md), [DragLeave](uielement_dragleave.md), [DragOver](uielement_dragover.md), and [Drop](uielement_drop.md) events of a [UIElement](uielement.md).

## -parameters

### -param sender
The object where the event handler is attached.

### -param e
The event data.


## -remarks
[DragEventHandler](drageventhandler.md) is the delegate you implement to handle these events:
+ [UIElement.DragEnter](uielement_drop.md)
+ [UIElement.DragLeave](uielement_dragleave.md)
+ [UIElement.DragOver](uielement_dragover.md)
+ [UIElement.Drop](uielement_drop.md)
These events are routed events. Changing the value of the [Handled](drageventargs_handled.md) property of [DragEventArgs](drageventargs.md) from an event handler can influence how a routed event behaves. For more info on the routed event concept, see [Events and routed events overview](http://msdn.microsoft.com/library/34c219e8-3efb-45bc-8bbd-6fd937698832).

The [Control](../windows.ui.xaml.controls/control.md) class has pre-wired event handlers that [Control](../windows.ui.xaml.controls/control.md) derived types can override to provide class-based handling for the drag-drop events,. These methods are:
+ [Control.OnDragEnter](../windows.ui.xaml.controls/control_ondragenter.md)
+ [Control.OnDragLeave](../windows.ui.xaml.controls/control_ondragleave.md)
+ [Control.OnDragOver](../windows.ui.xaml.controls/control_ondragover.md)
+ [Control.OnDrop](../windows.ui.xaml.controls/control_ondrop.md)


The Windows Runtime implementation of drag-drop concepts permits only certain controls and input actions to initiate a drag-drop action. There is no generalized **DoDragDrop** method that would permit any UI element to initiate a drag-drop action. The main source of a drag-drop action is when you drag the items of a list such as [GridView](../windows.ui.xaml.controls/gridview.md). 
<!--TODO is there any conceptual on drag drop and design for interaction that is not tainted with CSS and JS concepts?-->

## -examples

## -see-also
[Events and routed events overview](http://msdn.microsoft.com/library/34c219e8-3efb-45bc-8bbd-6fd937698832), [DragEventArgs](drageventargs.md)