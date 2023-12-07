# ⚙ Konfiguration Qwiic OpenLog

Ich habe den Modus des Qwiic OpenLog in der config.txt auf seiner SD-Karte von MODE\_NEWLOG auf MODE\_SEQLOG geändert, damit nicht immer automatisch eine neue Log-Datei angelegt wird. Die automatisch angelegte Log-Datei möchte ich nicht verwenden. Ich lege meine Log-Dateien lieber selbst an.

{% code title="config.txt" %}
```
42,26,3,1
i2c_address,escape,esc#,mode

```
{% endcode %}
