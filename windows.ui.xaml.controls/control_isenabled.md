---
-api-type: winrt property
---
 The control can't receive keyboard focus or be focused programmatically.
 The control does not appear in a tab sequence (any value for [TabIndex](control_tabindex.md) is ignored).
 A disabled control is still visible to hit testing. It can't handle any input events on itself. However, a disabled control can still source the input events, and input routed events can bubble to a parent where they can be handled.