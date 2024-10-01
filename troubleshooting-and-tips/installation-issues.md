# Installation Issues

## Windows Installation Issues

{% hint style="danger" %}
* The most common mistake is putting a **plugin in the wrong folder.**
* Make sure that you are installing **64-bit plugins** if you are on the 64-bit platform.&#x20;
* **Pro Tools**: Sometimes AAX plugin could not be loaded. This could happen if the plugin signature is broken. Delete the old plugin and install it again to solve the issue.&#x20;
* **Ableton Live**: Make sure to enable plugins in the settings.&#x20;
{% endhint %}

***

## macOS Installation Issues

{% hint style="danger" %}
* The most common issue happens if you **overwrite the old plugin** when upgrading. Make sure to delete the old plugins before copying the new ones.&#x20;
* Usually **logging off or rebooting** is required after manual installation.
* If the plugin can not be found, or the app cannot be opened, you might need an **older version**. Please [contact us.](https://youlean.co/contact/)
{% endhint %}

### Fixing Audio Unit Issues

Delete the old plugin and then copy a new one. Log off, or reboot your Mac if the plugin can not be loaded.

If you want to manually validate the Audio Unit, open the **"Terminal"** application and run this command:

```
auval -v aufx urbY gtuY
```

For more advanced troubleshooting methods run these commands in **"Terminal"**:

{% hint style="info" %}
**This is a safe operation**

This will kill AudioComponentRegistrar process.&#x20;

It could solve the Audio Unit not showing up problem.

{% code title="Command:" %}
```
killall -9 AudioComponentRegistrar
```
{% endcode %}
{% endhint %}

{% hint style="info" %}
**This is a safe operation**

Delete **com.apple.audio.InfoHelper.plist** file. This could be done using Finder or Terminal via the command below.

It could solve various Audio Unit issues.

{% code title="Command:" %}
```
rm ~/Library/Preferences/com.apple.audio.InfoHelper.plist
```
{% endcode %}
{% endhint %}

{% hint style="warning" %}
**Warning**

Delete **com.apple.audiounits.cache** file. This could be done using Finder or Terminal via the command below.

It will force a full rescan of all Audio Units on your system.&#x20;

It could solve various Audio Unit issues.

{% code title="Command:" %}
```
rm ~/Library/Caches/AudioUnitCache/com.apple.audiounits.cache
```
{% endcode %}
{% endhint %}

{% hint style="danger" %}
**Unsafe. Do only as a last resort**&#x20;

Delete **com.apple.logic10.plist** file. This could be done using Finder or Terminal via the command below.

It will reset all Logic Pro X settings.&#x20;

Most commonly it will solve issues where a plugin is not available in some channel configurations.

{% code title="Command:" %}
```
rm ~/Library/Preferences/com.apple.logic10.plist
```
{% endcode %}
{% endhint %}
