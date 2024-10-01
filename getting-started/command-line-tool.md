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
