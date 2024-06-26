![ring-mqtt-logo](https://raw.githubusercontent.com/PatrickSt1991/ring-mqtt-v2/main/images/github.jpg)

## Credits where credits are due
As this is a fork of tsightler, all credits must go to him and the people who helped in the original project.

I only created a new feature that suited my requirements, it couldn't be merged in to the original repo so that's why I continued on my own fork.

As this fork contains much of the original code, i did my best to make this repo stand on it's own.

***Please feel free to update the code or fork it to you're own***

## About
Ring LLC sells security related products such as video doorbells, security cameras, alarm systems and smart lighting devices.  The ring-mqtt project uses the Ring API (the same one used by Ring official apps) to act as a bridge between these devices and an local MQTT broker, thus allowing any automation tools that can leverage the open standards based MQTT protocol to effectively integrate with these devices.  The project also supports video streaming by providing an RTSP gateway service that allows any media client supporting the RTSP protocol to connect to a Ring camera livestream or to play back recorded events (Ring Protect subscription required for event recording playback).  Please review the full list of [supported devices and features](https://github.com/PatrickSt1991/ring-mqtt-v2/wiki#supported-devices-and-features) for more information on current capabilities.

#### IMPORTANT NOTE - Please read
Ring devices are sold as cloud based devices and this project uses the same cloud based API used by the Ring apps, it does not enable local control of Ring devices as there is no known facility to do so.  While using this project does not technically require a Ring Protect subscription, many capabilities are not possible without a subscription and this project is not intended as a way to bypass this requirement.  If you don't like cloud powered devices my suggestion is to not purchase them.

Also, this project does not turn Ring video doorbells/cameras into 24x7/continuous streaming CCTV cameras as these devices are designed for event based streaming/recording or for light interactive viewing, such as answering the a doorbell ding, or checking on a motion event.  Even when using this project, all streaming still goes through Ring cloud servers and is not local.  Attempting to leverage this project for continuous streaming is not a supported use case and attempts to do so will almost certainly end in disappointment, this includes use with NVR tools like Frigate, Zoneminder or others.

If this advice is ignored, please note that there are significant functional side effects to doing so, most notably loss of motion/ding events while streaming (Ring cameras will only send alerts when they are not actively streaming/recording), quickly drained batteries, and potential device overheating or even early device failure as Ring cameras simply aren't designed for continuous operation.  While you are of course welcome to use this project however you like, questions about use of tools that require continuous streaming will be locked and deleted.

## Installation and Configuration
Please refer to the [ring-mqtt project wiki](https://github.com/PatrickSt1991/ring-mqtt-v2/wiki) for complete documentation on the various installation methods and configuration options.
