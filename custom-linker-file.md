# 💻 Custom Linker File

Original Linker File wurde duch custom Linker File ersetzt, um die RAM-Nutzung durch "default" FASTRUN Code zu reduzieren, vor allem von der Bibliothek ESP-Mail-Client.\
Zur Erläuterung: "normaler" Code wird zum Teil neben explizitem FASTRUN Code beim Start des Mikrocontrollers in den RAM geladen, um schneller ausgeführt zu werden. Die ESP-Mail-Client Bibliothek verursachte dies im großem Umfang: ca. 350 kbyte!

Pfad zum Linker File: "%AppData%\Local\Arduino15\packages\teensy\hardware\avr\\%VERSION%\cores\teensy4"

(siehe [https://forum.pjrc.com/index.php?threads/flashmem-for-all-functions-in-a-file.69185/#post-302633](https://forum.pjrc.com/index.php?threads/flashmem-for-all-functions-in-a-file.69185/#post-302633))

{% file src=".gitbook/assets/imxrt1062_t41.ld" %}
Costum Linker File
{% endfile %}

{% file src=".gitbook/assets/imxrt1062_t41_ORIGINAL.ld" %}
Original Linker File
{% endfile %}



