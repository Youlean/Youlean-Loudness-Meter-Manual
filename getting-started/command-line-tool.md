# Command-Line Tool

The Command-Line Tool of Youlean Loudness Meter 2 offers advanced users an efficient way to analyze and normalize audio files, and export reports. To begin using the tool, ensure it's properly installed. You can either manually install it or use an installer to integrate it into your system path for system-wide availability.

**Basic Usage:**

The tool functions via specific command line arguments. Here's the basic usage structure:

```bash
Usage: --input-file-path <path> [options]
```

{% hint style="info" %}
Always use absolute paths as relative paths are not supported.
{% endhint %}

**Key Commands and Options:**

* `--input-file-path <path>`: Sets the input file path. You can input multiple paths for multi-mono files.
* `--preset-name <name>`: Selects the preset name for analysis settings.
* `--channel-config <config>`: Chooses the channel configuration, with 'auto' as the default.
* `--export`: Triggers the export of reports.
* `--normalize`: Exports a normalized file.

**Examples of Usage:**

1. **Basic Analysis**:

{% code overflow="wrap" %}
```bash
--input-file-path "/your/file/path/file.wav"
```
{% endcode %}

{% hint style="info" %}
You can also analyze multi-mono files too:

```
ylm2 --input-file-path "C:\example\file.L.wav" "C:\example\file.R.wav" "C:\example\file.C.wav" "C:\example\file.LFE.wav" "C:\example\file.Ls.wav" "C:\example\file.Rs.wav"
```
{% endhint %}

This command analyzes the specified file and prints the results.

2. **Analysis with Export**:

{% code overflow="wrap" %}
```bash
--input-file-path "/your/file/path/file.wav" --export --export-type "PNG"
```
{% endcode %}

Analyzes the file and exports the results as a PNG.

3. **Normalization and Export**:

{% code overflow="wrap" %}
```bash
--input-file-path "/your/file/path/file.wav" --normalize --export --export-type "PDF"
```
{% endcode %}

Normalizes the audio file and exports a PDF report.

{% hint style="info" %}
**Tips for Effective Use:**

* **Preset Selection**: Use the Youlean Loudness Meter 2 application to create and select presets with desired settings for your analysis.
* **Export Customization**: Customize your export options (type, folder path, file name) based on your requirements.
* **Console Results**: Use `--print-result` to see immediate analysis results in the console.
* For a full list of `--preset-name`, `--channel-config`, and `--export-type` options, use `--help` to print options to the console.
{% endhint %}

#### Examples

You can download the scripts here and double-click on the script to load it. On macOS, you may need to make the script executable by using `chmod +x`. Once launched, it will prompt you to specify the folder for analysis. You can drag the folder from File Explorer or Finder, and every audio file will be analyzed, generating a report.

{% embed url="https://youlean.co/wp-content/uploads/2025/10/ylm2-Analyze-Folder.zip" %}

To automatically organize your files during processing, the script will create three folders:

* `ylm2-to-process`: This directory is monitored for new files to be analyzed.
* `ylm2-completed`: Successfully processed files are moved here.
* `ylm2-failed`: Files that fail to process are moved to this folder.

Insert files into the `ylm2-to-process`, and the script will handle them based on the outcome of the analysis.

{% embed url="https://youlean.co/wp-content/uploads/2025/10/ylm2-Batch-Process-Analyze.zip" %}
