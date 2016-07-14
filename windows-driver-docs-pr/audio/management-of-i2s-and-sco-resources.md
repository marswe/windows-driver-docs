---
Description: 'The Management of I2S and SCO Resources topic discusses the assumptions that were made in the design of this new support for Bluetooth bypass audio streaming in Windows 8.1.'
MS-HAID: 'audio.management\_of\_i2s\_and\_sco\_resources'
MSHAttr: 'PreferredLib:/library/windows/hardware'
title: Management of I2S and SCO Resources
---

# Management of I2S and SCO Resources


The Management of I2S and SCO Resources topic discusses the assumptions that were made in the design of this new support for Bluetooth bypass audio streaming in Windows 8.1.

At this time Windows assumes that there is only one Bluetooth host controller. And also, the HFP synchronous connection oriented (SCO) bypass support assumes that there is only one bypass connection and that, any channel opened through the HFP device driver interface is associated with that single connection.

Audio drivers should arbitrate this channel and the single bypass connection for a single consumer on a first-come first-serve basis. The simplest way to achieve this is for the driver to allow only a single filter to transition its pins to the ACQUIRE state.

## <span id="related_topics"></span>Related topics


[Theory of Operation](theory-of-operation.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[audio\audio]:%20Management%20of%20I2S%20and%20SCO%20Resources%20%20RELEASE:%20%287/14/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/en-us/default.aspx. "Send comments about this topic to Microsoft")



