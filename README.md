# VTT to Text Converter

A browser-based tool that converts VTT (WebVTT) subtitle files to plain text format with smart consolidation of segments. Built with vanilla JavaScript and styled using Tailwind CSS.

## Features

- 🚀 Live Conversion: Real-time VTT to text conversion as you type or paste
- ⌛ Smart Consolidation: Automatically groups subtitles into ~20-second segments
- ⚡ Accurate Parsing: Correctly handles VTT timestamps and multi-line subtitles
- 📋 Easy Export: Copy to clipboard or download as text file
- 🎨 Modern Interface: Clean, responsive design with intuitive controls
- ⌨️ Keyboard Accessible: Full keyboard navigation support
- 📱 Mobile Friendly: Responsive design that works on all devices

## Usage

1. Open `index.html` in a modern web browser
2. Paste your VTT content into the input area
3. The converted text appears automatically in the output area
4. Use the Copy or Download buttons to export the result

### Input Format (VTT)
```
WEBVTT

00:00:00.000 --> 00:00:05.000
First subtitle line

00:00:05.000 --> 00:00:10.000
Second subtitle line
```

### Output Format
```
[00:00:00.000 --> 00:00:10.000] First subtitle line Second subtitle line
[00:00:10.000 --> 00:00:20.000] Next group of subtitle lines consolidated together
```

The converter automatically groups subtitles into approximately 20-second segments, making the transcript more readable.

## Technical Details

- Pure JavaScript implementation with no backend dependencies
- Intelligent subtitle consolidation algorithm for better readability
- Uses the Lucide icon library for UI elements
- Tailwind CSS for styling
- Regular expressions for accurate timestamp parsing
- Blob API for file downloads
- Clipboard API for copy functionality

## Browser Support

Supports all modern browsers including:
- Chrome
- Firefox
- Safari
- Edge

## Performance

The converter handles VTT files efficiently with:
- Immediate conversion feedback
- Optimized regex pattern matching
- Minimal DOM operations
- Error handling for invalid inputs

## Development

To modify the project:
1. Clone the repository
2. Edit the `index.html` file
3. Test in a browser (no build step required)

### Code Structure

- HTML: Contains the structure and inline JavaScript
- CSS: Tailwind utility classes with custom styles
- JavaScript: Event handlers and conversion logic

## License

MIT License