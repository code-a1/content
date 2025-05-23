---
title: "Window: deviceorientationabsolute event"
short-title: deviceorientationabsolute
slug: Web/API/Window/deviceorientationabsolute_event
page-type: web-api-event
browser-compat: api.Window.deviceorientationabsolute_event
---

{{APIRef("Device Orientation Events")}}{{securecontext_header}}

The **`deviceorientationabsolute`** event is fired when absolute device orientation changes.

This event is not cancelable and does not bubble.

## Syntax

Use the event name in methods like {{domxref("EventTarget.addEventListener", "addEventListener()")}}, or set an event handler property.

```js-nolint
addEventListener("deviceorientationabsolute", (event) => { })

ondeviceorientationabsolute = (event) => { }
```

## Event type

A {{domxref("DeviceOrientationEvent")}}. Inherits from {{domxref("Event")}}.

{{InheritanceDiagram("DeviceOrientationEvent")}}

## Event properties

- {{domxref("DeviceOrientationEvent.absolute")}} {{ReadOnlyInline}}
  - : A boolean that indicates whether the device is providing orientation data absolutely.
- {{domxref("DeviceOrientationEvent.alpha")}} {{ReadOnlyInline}}
  - : A number representing the motion of the device around the z axis, expressed in degrees with values ranging from 0 (inclusive) to 360 (exclusive).
- {{domxref("DeviceOrientationEvent.beta")}} {{ReadOnlyInline}}
  - : A number representing the motion of the device around the x axis, expressed in degrees with values ranging from -180 (inclusive) to 180 (exclusive). This represents a front to back motion of the device.
- {{domxref("DeviceOrientationEvent.gamma")}} {{ReadOnlyInline}}
  - : A number representing the motion of the device around the y axis, expressed in degrees with values ranging from -90 (inclusive) to 90 (exclusive). This represents a left to right motion of the device.
- `DeviceOrientationEvent.webkitCompassHeading` {{Non-standard_Inline}} {{ReadOnlyInline}}
  - : A number represents the difference between the motion of the device around the z axis of the world system and the direction of north, expressed in degrees with values ranging from 0 to 360.
- `DeviceOrientationEvent.webkitCompassAccuracy` {{Non-standard_Inline}} {{ReadOnlyInline}}
  - : The accuracy of the compass given as a positive or negative deviation. It's usually 10.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- {{DOMxRef("window.devicemotion_event", "devicemotion")}} event
- {{DOMxRef("window.deviceorientation_event", "deviceorientation")}} event
- [Detecting device orientation](/en-US/docs/Web/API/Device_orientation_events/Detecting_device_orientation)
