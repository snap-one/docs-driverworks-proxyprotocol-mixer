# Introduction

### Lua Mixer Proxy

_Note: The Mixer Proxy is the first Lua Proxy delivered by Control4. The architecture used to develop this proxy is not currently available to third party developers. Furthermore, drivers developed using the Lua Proxy methodology lack a user interface which is typically provided for a driver written using  Control4’s traditional, non-Lua proxies. Control4 is not in a position to provide user interfaces for third party drivers written using a Lua proxy._

The Mixer proxy is intended to be used in conjunction with the [AV Switch proxy][1]. The AV Switch proxy handles all the typical AV Switch functions such as input/output selection, room/zone volume control, etc. The Mixer proxy extends this functionality to support Mixer channel volume/mute control as well as Digital Signal Processing (DSP). 

In addition to the normal AV Switch constructs of Inputs, Outputs and Selected Source the Mixer proxy adds Channels, Zones and Mixes. Channels also support advanced DSP signal processing including EQ, Compression, De-Essing and Noise Gate.

AV Pathing and Source selection are at the heart of most AV proxies and the Mixer proxy is no different. However, since the Mixer proxy is designed to extend the AV Switch proxy, some of these lines do get blurred. For example, a CD player bound to an input of the protocol driver is part of the AV Switch pathing logic but it is also a channel of the Mixer and as such can be part of a Mix.

Furthermore, it may be desired to start an audio session by just selecting a Mix of channels and not have a particular selected (controllable) source. Or the user may wish to select a single microphone (not controllable) as the selected source. To handle these use cases, No Control drivers have been created for both Microphone and Mix.

Since Mixes and Channels require different handling logic, the Mixer proxy must know if the selected source is a Channel or a Mix. To support this functionality, special mixId and channelId elements must be included in the appropriate Input Connections in the protocol driver. Using this modeling, the Proxy maintains a map of all connections with this data in the MIXER\_CONNECTIONS table.

An important distinction (and possible source of confusion) is how the UI and Proxy handle Input Channel Volume. As in the case of actual mixer devices, an input channel has a level (volume) control which will affect the signal before any further modification of that channel in a mix. For example, if a device can create more than one mix, changing the input channel volume will affect the level of that channel in all mixes. Whereas changing the volume of that channel in a mix will only affect the level of that channel in that mix. While this is a straightforward concept, it does get clouded by Control4 source selection and control logic in conjunction with the fact that the mixer proxy is the first AV Proxy that handles volume control of an input (Room volume control adjusts the volume of an output/zone in a device). To simplify user interaction, it has been decided that, from a Control4 perspective, Input Channel Level will be a configuration element and not supported via the Control4 UI. So, when a Source is selected, the level control is visible but grayed out and not available for modification. When a Mix is selected, all Channels are available for modification in that Mix.

**Channel Selected**
<img src="images/mixerproxy001.jpg"/>

**Mix Selected**
<img src="images/mixerproxy002.jpg"/>

**Minimum Requirements**

- Composer Pro: 4.1.0
- Director version: 4.0.0

[1]:	https://snap-one.github.io/docs-driverworks-proxyprotocol-avswitch/#license-copyright-and-trademark