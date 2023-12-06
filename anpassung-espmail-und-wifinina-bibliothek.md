# ⛓ Anpassung ESPMail- und WiFiNINA-Bibliothek

Die Adafruit WiFiNINA Bibliothek hat kein WiFi disconnect, daher darf ESP\_MAIL\_HAS\_WIFI\_DISCONNECT nicht definiert sein.

Um das zu erreichen wird in WiFiNINA.h (Adafruit WiFiNINA) ADAFRUIT\_WIFI\_NINA definiert und in Networks.h (ESPMail) geprüft, ob es definiert ist.

{% code title="WiFiNINA.h" %}
```cpp
#ifndef WiFiNINA_h
#define WiFiNINA_h

#define ADAFRUIT_WIFI_NINA

#include "WiFi.h"

#endif
```
{% endcode %}

{% code title="Networks.h" %}
```cpp
#if !defined(ARDUINO_RASPBERRY_PI_PICO_W) && \
...
    !defined(ADAFRUIT_WIFI_NINA)
#define ESP_MAIL_HAS_WIFI_DISCONNECT
#endif
```
{% endcode %}
