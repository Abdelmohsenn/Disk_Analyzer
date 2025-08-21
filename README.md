# Disk_Analyzer with Tauri
Rust + React with Tauri Linking

A fast desktop application built with **Tauri** and **Rust** for analyzing disk usage and managing files.

## Features

- **📁 Directory Analysis**: Scan directories and calculate sizes recursively
- **🔍 Find Largest Files**: Identify top 5 largest files in any directory  
- **📊 Multiple Size Units**: Display in Bytes, KB, MB, and GB
- **🗑️ File Management**: Delete and copy files directly
- **📤 Export Data**: Save analysis results to text files
- **⚡ High Performance**: Parallel processing with Rust backend

## Tech Stack

- **Backend**: Rust with Tauri framework
- **Parallel Processing**: Rayon for concurrent file operations
- **Frontend**: Tauri webview interface
- **File System**: WalkDir for efficient directory traversal

## Quick Start

```bash
# Clone and install
https://github.com/Abdelmohsenn/Disk_Analyzer.git
cd Disk_Analyzer
cargo build

# Development
cargo tauri dev

# Build for production
cargo tauri build
```

## Main Commands

```rust
store_directories(path)     // Analyze directory sizes
scan_largest(path)          // Find 5 largest files
save_data_to_file()         // Export results
delete_file(path)           // Remove files
copy_contents(src, dest)    // Copy files
```

## Key Features

- **Cross-platform** (Windows, macOS, Linux)
- **Memory efficient** with streaming large directories
- **Native performance** through Rust backend
- **Responsive UI** with non-blocking operations

## Dependencies

```toml
tauri = "1.0"
rayon = "1.7"        # Parallel processing
walkdir = "2.3"      # Directory traversal
serde = "1.0"        # Serialization
```

---

**Built with Rust + Tauri for native performance and modern UI**
