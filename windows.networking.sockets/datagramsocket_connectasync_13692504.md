---
-api-type: winrt method
---
 Using one of the [GetOutputStreamAsync](datagramsocket_getoutputstreamasync.md) methods.
 After a successful call to the [ConnectAsync](datagramsocket_connectasync_13692504.md) method using the [OutputStream](datagramsocket_outputstream.md) property.
 Create the [DatagramSocket](datagramsocket.md).
 Use the [Control](datagramsocket_control.md) property on the [DatagramSocket](datagramsocket.md) to retrieve a [DatagramSocketControl](datagramsocketcontrol.md) object and set any advanced controls. This step is not normally needed by most apps.
 Assign the [MessageReceived ](datagramsocket_messagereceived.md) event to an event handler.
 Call the [ConnectAsync](datagramsocket_connectasync_1841953676.md) method to connect to the remote endpoint.
 Use the [OutputStream](datagramsocket_outputstream.md) property on the [DatagramSocket](datagramsocket.md) with a [DataWriter](../windows.storage.streams/datawriter.md) object to send messages to the remote endpoint.
 The [MessageReceived](datagramsocket_messagereceived.md) event handler will be invoked whenever a message from the remote endpoint arrives.