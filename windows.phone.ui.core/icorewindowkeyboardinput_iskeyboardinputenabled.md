---
-api-type: winrt property
---
 1. You use the default buffer. (For example, you do not provide your own [KeyboardInputBuffer](../windows.ui.core/corewindow_keyboardinputbuffer.md).)
 2. You programmatically open the touch keyboard by setting [IsKeyboardInputEnabled](../windows.ui.core/corewindow_iskeyboardinputenabled.md) to true.
 3. The user presses the back button, which closes the touch keyboard.
 4. You read [IsKeyboardInputEnabled](../windows.ui.core/corewindow_iskeyboardinputenabled.md) and expect the value to be false (since the touch keyboard was closed), but the value is true.
 Do not use the default buffer.
 Do not use [IsKeyboardInputEnabled](../windows.ui.core/corewindow_iskeyboardinputenabled.md).
 Listen to the [Hiding](../windows.ui.viewmanagement/inputpane_hiding.md) event and set [IsKeyboardInputEnabled](../windows.ui.core/corewindow_iskeyboardinputenabled.md) to false.
 Use the [OccludedRect](../windows.ui.viewmanagement/inputpane_occludedrect.md) property to see if the touch keyboard is open.