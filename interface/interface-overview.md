# Interface Overview

<figure><img src="../.gitbook/assets/Youlean Loudness Meter 2.png" alt=""><figcaption></figcaption></figure>

***

## Channel Configuration&#x20;

<div align="left">

<figure><img src="../.gitbook/assets/Channel Configuration.png" alt="" width="210"><figcaption></figcaption></figure>

</div>

Use this dropdown menu to change the channel configuration.

{% hint style="info" %}
Configurations marked with **(A)** indicate an automatic recognition by the system. You can rely on these settings for standard operations, but adjustments can be made from the dropdown menu if necessary.
{% endhint %}

***

## Presets

<div align="left">

<figure><img src="../.gitbook/assets/Presets.png" alt="" width="298"><figcaption></figcaption></figure>

</div>

Use this dropdown menu to change the meter preset.

{% hint style="info" %}
Presets marked with an asterisk (**\***) indicate that the settings have been modified from their initial state.
{% endhint %}

***

<div align="left">

<figure><img src="../.gitbook/assets/Presets - Set Default.png" alt="" width="375"><figcaption></figcaption></figure>

</div>

To set a preset as the default, simply click the **"Set Default"** option in the dropdown menu. Once you've set a preset as your default, it will automatically load each time the meter is loaded, ensuring a consistent setup tailored to your preferences.

***

<div align="left">

<figure><img src="../.gitbook/assets/Presets - Import.png" alt="" width="375"><figcaption></figcaption></figure>

</div>

To import a preset, navigate to the **"Import"** option in the dropdown menu and select the file you wish to import. This allows you to quickly apply configurations from previously saved presets, streamlining your setup process.

***

<div align="left">

<figure><img src="../.gitbook/assets/Presets - Save.png" alt="" width="375"><figcaption></figcaption></figure>

</div>

Click "**Save Preset"** to store your current settings for future use, ensuring easy access and application of your preferred configurations.

{% hint style="info" %}
Saved presets encompass all meter settings, including GUI size, to ensure consistent loading of necessary configurations across different systems.
{% endhint %}

***

<div align="left">

<figure><img src="../.gitbook/assets/Preset Info.png" alt="" width="375"><figcaption></figcaption></figure>

</div>

Hover your mouse over the **"i"** button to preview the current preset alerts and targets.

***

## Pause Measurements

<div align="left">

<figure><img src="../.gitbook/assets/Pause Measurements Button.png" alt="" width="136"><figcaption></figcaption></figure>

</div>

Click here to pause all measurements.

{% hint style="info" %}
After file analysis or normalization, measurements will be paused automatically.&#x20;
{% endhint %}

***

<div align="left">

<figure><img src="../.gitbook/assets/Pause INT-LRA Button.png" alt="" width="206"><figcaption></figcaption></figure>

</div>

Click here to pause integrated loudness and loudness range measurements.&#x20;

***

<div align="left">

<figure><img src="../.gitbook/assets/Reset Button.png" alt="" width="201"><figcaption></figcaption></figure>

</div>

Click here to clear all measurements.

***

<div align="left">

<figure><img src="../.gitbook/assets/Auto Reset Button.png" alt="" width="228"><figcaption></figcaption></figure>

</div>

**"AUTO"** button will control if measurements will be cleared automatically once host starts playing.

{% hint style="info" %}
This button will be disabled when **"Continuous"** histogram mode is active because automatic measurement resets are not supported there.&#x20;
{% endhint %}

***

## Meter Bars

<div align="left">

<figure><img src="../.gitbook/assets/Meter Bar Momentary.png" alt="" width="171"><figcaption></figcaption></figure>

</div>

Three different styles of meter bars are available. In this style, the bar displays momentary loudness, while a triangle indicates short-term loudness.

***

<div align="left">

<figure><img src="../.gitbook/assets/Meter Bar Momentary, Short Term.png" alt="" width="184"><figcaption></figcaption></figure>

</div>

Here the left indicates momentary loudness, and the right displays short-term loudness.

***

<div align="left">

<figure><img src="../.gitbook/assets/Meter Bar Momentary, Dynamics, Short Term.png" alt="" width="171"><figcaption></figcaption></figure>

</div>

Here the left indicates momentary loudness, middle one indicated dynamics, and the right displays short-term loudness.

***

<div align="left">

<figure><img src="../.gitbook/assets/Meter Loudness Range.png" alt="" width="92"><figcaption></figcaption></figure>

</div>

This is the loudness range indicator.&#x20;

## Peak Meters

<div align="left">

<figure><img src="../.gitbook/assets/Peak Meters.png" alt="" width="289"><figcaption></figcaption></figure>

</div>

In the [View Menu](../settings-and-menus/meter-menus/view-menu.md) you can enable true peak meters. Peak meters channel configuration will be adjusted automatically based on the channel settings.&#x20;

{% hint style="info" %}
You can show all peak meters even if your channel configuration is for example mono. That could help you detect if the audio is coming from channel that is not included in the current channel configuration. This setting can be changed in the [View Menu.](../settings-and-menus/meter-menus/view-menu.md)&#x20;
{% endhint %}

***

## Numerical Readouts



<div align="left">

<figure><img src="../.gitbook/assets/Integrated Loudness.png" alt="" width="333"><figcaption></figcaption></figure>

</div>

The numerical displays will provide the current measurements.

{% hint style="info" %}
If the last 3 seconds of analysis are silent, dynamics and short-term measurements may be invalid. This occurs because these measurements are real-time and reflect only the most recent audio.
{% endhint %}

***

<div align="left">

<figure><img src="../.gitbook/assets/Integrated Loudness Warning Under.png" alt="" width="333"><figcaption></figcaption></figure>

</div>

If the measurement is below its target, it will be shown as orange.

***

<div align="left">

<figure><img src="../.gitbook/assets/Integrated Loudness Warning Over.png" alt="" width="333"><figcaption></figcaption></figure>

</div>

If the measurement is above its target, it will be shown as red.&#x20;

{% hint style="info" %}
You can set measurement targets in the [Settings Menu. ](../settings-and-menus/meter-menus/settings-menu.md)
{% endhint %}

***

<div align="left">

<figure><img src="../.gitbook/assets/True Peak Reset.png" alt="" width="333"><figcaption></figcaption></figure>

</div>

You can reset some measurements by clicking on it.&#x20;

***

<div align="left">

<figure><img src="../.gitbook/assets/True Peak Clipping Indicators.png" alt="" width="333"><figcaption></figcaption></figure>

</div>

True peak measurement will show you the channels where value was above the target.&#x20;

***

## A/B State

<div align="left">

<figure><img src="../.gitbook/assets/A,B States.png" alt="" width="254"><figcaption></figcaption></figure>

</div>

