---
-api-id: T:Windows.Devices.Sensors.Inclinometer
-api-type: winrt class
---

<!-- Class syntax.
public class Inclinometer : Windows.Devices.Sensors.IInclinometer, Windows.Devices.Sensors.IInclinometer2, Windows.Devices.Sensors.IInclinometerDeviceId
-->

# Windows.Devices.Sensors.Inclinometer

## -description

Represents an inclinometer sensor.

This sensor returns pitch, roll, and yaw values that correspond to rotation angles around the x, y, and z axes, respectively.

For an example implementation, see the inclinometer sample [https://github.com/Microsoft/Windows-universal-samples/tree/master/Samples/Inclinometer](https://github.com/Microsoft/Windows-universal-samples/tree/master/Samples/Inclinometer).

## -remarks

Sensor data is provided relative to the device's fixed sensor coordinate system, and is independent of display orientation. For applications that rely on sensor data for input control or to manipulate elements on the screen, the developer must take current display orientation into account and compensate the data appropriately. For more info about the sensor coordinate system, see [Sensor data and display orientation](https://msdn.microsoft.com/library/f90937f1-edaf-469c-b360-2ed67cb4fad0).

The following example demonstrates how a UWP app built with XAML and C# uses the [GetDefault](inclinometer_getdefault_2064571144.md) method to establish a connection to an inclinometer. If no integrated inclinometer is found, the method will return a null value.

[!code-csharp[GetDefaultCS](../windows.devices.sensors/code/inclinometer/csharp/Scenario1.xaml.cs#SnippetGetDefaultCS)]

The following example demonstrates how a UWP app built with XAML registers a [ReadingChanged](inclinometer_readingchanged.md) event handler.

[!code-csharp[EnableReadingChangedCS](../windows.devices.sensors/code/inclinometer/csharp/Scenario1.xaml.cs#SnippetEnableReadingChangedCS)]

The following example shows the [ReadingChanged](inclinometer_readingchanged.md) event handler.

[!code-csharp[ReadingChangedCS](../windows.devices.sensors/code/inclinometer/csharp/Scenario1.xaml.cs#SnippetReadingChangedCS)]

## -examples

## -see-also

[Inclinometer Sample](https://go.microsoft.com/fwlink/p/?linkid=241380), [Sensor data and display orientation](https://msdn.microsoft.com/library/f90937f1-edaf-469c-b360-2ed67cb4fad0), [Inclinometer sample (Windows 10)](https://go.microsoft.com/fwlink/p/?LinkId=620552), [Relative inclinometer sample](https://github.com/Microsoft/Windows-universal-samples/tree/master/Samples/RelativeInclinometer)
