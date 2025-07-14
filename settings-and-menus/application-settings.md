# Application Settings

<figure><img src="../.gitbook/assets/YLM2 App Settings.png" alt=""><figcaption></figcaption></figure>

To access application settings to to **File->App Settings**

### Audio Device Settings

You can set here the audio device that meter should monitor.&#x20;

There are 3 main types of settings:

* **None** (audio driver is disabled)
* **Analyze Audio Inputs** (ASIO, DirectSound, Core Audio)
* **Analyze System Audio** (WASAPI, Core Audio)

### Audio Device Engine

* **Buffer Size:** It sets the internal buffer size for the meter.
* **Audio Sample Rate:** It is best to keep it at default so that the meter follows the current system sample rate
* **Audio Pass-Through:** If enabled, meter will pass input audio to the outputs

### Meter Input Channels

Here you should select the inputs for the meter. The order of inputs will matter. For example, if you want to measure stereo input, set **Input 1 to left** channels and **Input 2 to right** channel.&#x20;

### Application Window

Enable this to make meter always on top of other windows. This is useful if you want to have meter always visible while working on something else.&#x20;
