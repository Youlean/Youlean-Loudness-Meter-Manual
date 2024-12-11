# Common Issues and Solutions

## Plugin doesn't show in Ableton Live

Once you [install the VST3 plugin](../introduction/installation-windows.md) make sure that VST3 plugins are enabled in Ableton settings.&#x20;

<div align="left"><figure><img src="../.gitbook/assets/Ableton VST3 plugins.png" alt=""><figcaption></figcaption></figure></div>

For more info, [read Ableton's documentation.](https://help.ableton.com/hc/en-us/articles/209071729-Using-VST-plug-ins-on-Windows)

***

## Plugin and App Measurements are Different

The most likely cause for this issue could be:

* Wrong channel configuration
* The master channel fader is not at 0dB

***

## How to move all meter data to another computer

The user data is stored in the following locations:

**Windows:**

```
C:\Users\%USERNAME%\AppData\Local\Youlean\Youlean Loudness
```

**macOS:**

```
~/Library/Application Support/Youlean/Youlean Loudness Meter 2
```

To move all data, copy these folders to the other computers.

***

## The meter interface is not visible in Garageband

If you open a plugin and you see this:

<figure><img src="../.gitbook/assets/YLM2 Interface not visible Garageband.png" alt="" width="375"><figcaption></figcaption></figure>

Make sure that this option is disabled in Garageband preferences:

<figure><img src="../.gitbook/assets/YLM2 Interface not visible Garageband Fix.png" alt="" width="375"><figcaption></figcaption></figure>

***

## The meter doesn't show any measurements

The problem might be if the **Elapsed** histogram mode is selected, but audio playback is stopped.

The solution is to switch to continuous mode for measurements or to activate a host playback.
