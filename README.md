# Timeline Maker 📅

A powerful, feature-rich timeline creation tool built with React that allows you to create, manage, and share personal or professional timelines with file attachments, export capabilities, and timeline merging. Perfect for creating memory timelines, event timelines, and project timelines.

## ✨ Features

### 🎯 Core Timeline Creation
- **Create Timeline Entries**: Add memories, events, or milestones with dates and titles
- **File Attachments**: Attach images, PDFs, documents, videos, and other files to entries
- **Real-time Editing**: Click on titles to edit them inline
- **Automatic Sorting**: Entries are automatically sorted chronologically
- **Local Storage**: All data is saved locally in your browser

### 📤 Export & Import
- **Export as JSON**: Save timelines with rich metadata (name, description, date ranges)
- **Export as PDF**: Generate beautiful PDF documents of your timeline
- **Import Timelines**: Load previously exported timeline files
- **Backward Compatibility**: Supports both old and new export formats

### 🔀 Timeline Merging
- **Multi-file Selection**: Select multiple timeline files to merge
- **Merge Strategies**:
  - **Chronological**: Sort all entries by date across timelines
  - **By Source**: Group by original timeline, then sort by date
- **Live Preview**: See exactly how entries will be merged before confirming
- **Flexible Integration**: Choose to replace current timeline or add to it
- **Conflict Resolution**: Automatic ID collision handling

### 💾 File Management
- **Click-to-Download**: Click any attached file to download it instantly
- **Original Filenames**: Downloads preserve original filenames (e.g., `flight.pdf`, `vacation-photo.jpg`)
- **File Previews**: Hover over files to see previews and file information
- **Multiple File Types**: Support for images, PDFs, documents, videos, audio, archives
- **File Icons**: Visual indicators for different file types

### 🎨 User Interface
- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Modern UI**: Clean, intuitive interface with Tailwind CSS
- **Visual Timeline**: Alternating left/right layout with timeline nodes
- **Modal System**: Professional modals for export and merge operations
- **Hover Effects**: Smooth animations and visual feedback

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- No installation required - runs entirely in the browser

### Usage

1. **Open Timeline Maker**
   - Simply open `index.html` in your web browser
   - The application loads immediately with no setup required

2. **Create Your First Timeline Entry**
   - Select a date using the date picker
   - Enter a title for your memory/event
   - Click "Add Entry" to create your first timeline entry

3. **Attach Files to Your Timeline**
   - Click "📎 Add files" on any entry
   - Select one or more files (images, PDFs, documents, etc.)
   - Files are automatically attached and can be previewed

4. **Download Files from Your Timeline**
   - Hover over any attached file to see download hint
   - Click on the file to download it with its original filename
   - Files are downloaded directly to your device

## 📋 Detailed Feature Guide

### Creating Timeline Entries

```javascript
// Example timeline entry structure
{
  id: "unique_id",
  date: "2024-01-15",
  title: "Vacation to Paris",
  attachments: [
    {
      name: "eiffel-tower.jpg",
      type: "image/jpeg",
      size: 2048576,
      data: "data:image/jpeg;base64,...",
      safeFilename: "entry_id_0_eiffel-tower.jpg"
    }
  ]
}
```

### Exporting Timelines

**Export as JSON:**
1. Click "📤 Export Timeline"
2. Enter a name for your timeline (e.g., "vacation-2024")
3. Add an optional description
4. Click "Export Timeline"
5. File downloads as `vacation-2024.json`

**Export as PDF:**
1. Click "📄 Export PDF"
2. PDF is generated automatically with timeline layout
3. File downloads as `timeline_YYYY-MM-DD.pdf`

### Merging Timelines

1. Click "🔀 Merge Timelines"
2. Select multiple `.json` timeline files
3. Choose merge strategy:
   - **Chronological**: All entries sorted by date
   - **By Source**: Grouped by original timeline, then by date
4. Preview the merged result
5. Choose to replace current timeline or add to it

### File Management

**Supported File Types:**
- Images: JPG, PNG, GIF, WebP, etc.
- Documents: PDF, DOC, DOCX, TXT
- Videos: MP4, AVI, MOV, etc.
- Audio: MP3, WAV, etc.
- Archives: ZIP, RAR, etc.

**File Operations:**
- **Download**: Click any file to download with original filename
- **Preview**: Hover to see file information and previews
- **Remove**: Hover and click the × button to delete files

## 📄 License

This project is open source and available under the MIT License.

---

**Timeline Maker** - Create, manage, and share your memories with ease! 📅✨

Visit us at: [timelinemaker.site](https://timelinemaker.site)
