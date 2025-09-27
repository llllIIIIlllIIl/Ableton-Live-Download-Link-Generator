
# Ableton Download Link Generator

A clean, modern web application that generates official download links for Ableton Live directly from Ableton's CDN servers. Features dual CDN support and Ableton's signature grey aesthetic.

🌐 **Use Online**: [github.io hosted page](https://ableton-live.1113000.xyz/)


## ✨ Features

- **🔗 Dual CDN Support**: Primary and fallback download links from both `cdn-downloads.ableton.com` and `cdn2-downloads.ableton.com`
- **📦 Multiple Editions**: Support for Suite, Standard, Intro, Trial, and Lite editions
- **💻 Cross-Platform**: Generate download links for both Windows (.zip) and macOS (.dmg)
- **🧠 Version Intelligence**: Automatically handles architecture selection (64-bit vs Universal) based on version
- **🎨 Modern UI**: Clean, responsive design with Ableton's official grey color scheme
- **⚠️ User-Friendly**: Clear warnings about potential 404 errors and URL validation limitations

## 🚀 How to Use

### Quick Access (Recommended)
Simply visit: **[github.io hosted page](https://ableton-live.1113000.xyz/)**

1. Select your desired **Edition** (Suite is selected by default)
2. Choose your **Operating System** (Windows or macOS)
3. Enter the **Version Number** (e.g., 12.2.5)
4. Click "Generate Download Link" to get both primary and fallback download URLs

### Want to Customize?
If you want to modify the tool for your own needs:

1. **Download the HTML file**: Click on `index.html` in this repository, then click the "Download" button or right-click "Raw" → "Save as"
2. **Edit locally**: Open the downloaded file in any text editor
3. **Test**: Open the HTML file in your browser to test your changes
4. **Host**: Upload to your own web server or GitHub Pages

## 📋 Supported Versions

The generator works with Ableton Live versions that follow the standard URL pattern:
- **Live 11.1+**: Uses "universal" architecture for macOS
- **Live 11.0 and older**: Uses "64" architecture for all platforms
- **All versions**: Windows downloads use ".zip", macOS uses ".dmg"

### Version Examples:
- ✅ `12.2.5` 
- ✅ `11.0.12`
- ✅ `10.1.43`
- ✅  any version that really existed on their servers

## 🎯 URL Pattern

The generator creates URLs following Ableton's official CDN structure:

```
Primary:  https://cdn-downloads.ableton.com/channels/{version}/ableton_live_{edition}_{version}_{architecture}.{extension}
Fallback: https://cdn2-downloads.ableton.com/channels/{version}/ableton_live_{edition}_{version}_{architecture}.{extension}
```

### Examples:
- **Windows Suite**: `ableton_live_suite_12.2.5_64.zip`
- **macOS Suite (Modern)**: `ableton_live_suite_12.2.5_universal.dmg`
- **macOS Suite (Legacy)**: `ableton_live_suite_10.1.43_64.dmg`

## ⚠️ Important Notes

- **No URL Validation**: Due to CORS restrictions, the application cannot verify if download links exist before generation
- **Potential 404 Errors**: Invalid version numbers or discontinued versions may result in 404 errors
- **Dual CDN Strategy**: Two download options are provided to maximize success rate
- **Official Sources Only**: All links point to Ableton's official CDN servers

## 🛠️ Technical Details

- **Single HTML File**: Everything contained in one `index.html` file - no dependencies
- **Vanilla JavaScript**: No frameworks required, lightweight and fast
- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Modern CSS**: Glass morphism effects and smooth animations

## 📱 Browser Support

- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+


## 📄 License

Do anything you want
