The TouchLongPress event fires after a brief moment when the player holds their finger on the UI element using a touch-enabled device. It fires with a table of [DataType.Vector2](https://developer.roblox.com/search#stq=Vector2) that describe the relative screen positions of the fingers involved in the gesture. In addition, it fires multiple times with multiple [Enum.UserInputState](https://developer.roblox.com/search#stq=UserInputState)s: Begin after a brief delay, Change if the player moves their finger during the gesture and finally with End. The delay is platform dependent; in Studio it is a little longer than one second.

Since this event only requires one finger, this event can be simulated in Studio using the emulator and a mouse. Below is an example of TouchLongPress firing on a Frame that is [GuiObject.Active](https://developer.roblox.com/api-reference/property/GuiObject/Active). Below, the event fires after a brief delay (Begin) and then continually as as the finger is moved (Change). It fires one last time after it is released (End).

![TouchLongPress gesture][1]

This event is part of a family of touch-related events. Other events like this one are [GuiObject.TouchTap](https://developer.roblox.com/api-reference/event/GuiObject/TouchTap), [GuiObject.TouchRotate](https://developer.roblox.com/api-reference/event/GuiObject/TouchRotate), [GuiObject.TouchPinch](https://developer.roblox.com/api-reference/event/GuiObject/TouchPinch), [GuiObject.TouchPan](https://developer.roblox.com/api-reference/event/GuiObject/TouchPan) and [GuiObject.TouchSwipe](https://developer.roblox.com/api-reference/event/GuiObject/TouchSwipe). In addition, `UserInputService` has a similarly named event that is not restricted to a specific UI element: [UserInputService.TouchLongPress](https://developer.roblox.com/api-reference/event/UserInputService/TouchLongPress).

[1]: https://developer.roblox.com/assets/blt0bff2c10ae8eddd2/TouchLongPress.gif