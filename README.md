# My home assistant configuration

Here is my [home assistant}(https://home-assitant.io) configuration. I keep my configuration here as a backup as well as a source of inspiration for others. I regularly update this configuration, star it to keep up with the changes.

To check my current version of home assistant have a look [here](https://github.com/dasmaeh/ha-config/blob/master/.HA_VERSION).

I'll try to explain and document my setup here (short version) and at least some features at my [blog](https://dasmaeh.de/category/home-automation/).

## Host system
I'm running [hassOS](https://www.home-assistant.io/hassio/installation/) as a virtual machine using libvirt/qemu. So basically it's running hass.io in a VM instead of a Raspberry Pi, more or less because a virtual server host is running anyways at my home.
[Installation blog post](https://dasmaeh.de/2018/07/30/installation-of-hassos-libvirt/)

<!--()## Networking)-->
## Media players
At the moment: some SONOS PLAY:1 and PLAY:3 boxes.

<!--(
### MQTT Broker
To me [MQTT](https://www.home-assistant.io/components/mqtt) is one of the major communication protocols in home automation.
My MQTT broker is an [eclipse mosquitto](https://mosquitto.org/) instance running in a [docker container](https://hub.docker.com/_/eclipse-mosquitto/) in the DMZ of my home network. It is accessible on port 8883 (tls encrypted) from the internet and on port 8883 and 1883 (unencrypted) from inside my network. Unenecrypted access is necessary for my ESP8266 or ESP32 based DIY sensors.
TODO: Refernce to esphomeyaml, mqtt blog post, components

### Presence detection
Basically I'm using my wifes and my smartphone to detect who is home. Main source is [owntracks}(https://owntracks.org/). Owntracks alone has proven to be unrealiable at some occasions (my wife has a Huawei smartphone, known for their very aggressive battery opimizations and therefore sometime blocking owntracks). That's why I additionally use my WiFi accesspoint anf ping to track the phones.
These data are the statistically combined by bayes binary sensors.
TODO: links for components, blog post
)-->
