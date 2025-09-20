# 🎵 Music Automation System

An intelligent music collection system that automatically discovers, downloads, and organizes worship, gospel, and spiritual music from YouTube into your Jellyfin media library.

## ✨ Features

- **🤖 Automated Discovery**: Daily YouTube searches for worship, gospel, and spiritual music
- **📥 Smart Downloads**: Automatic audio extraction and organization
- **🎯 Jellyfin Integration**: Direct integration with Jellyfin media server
- **🔄 Duplicate Prevention**: Intelligent duplicate detection and prevention
- **📊 Analytics**: Download statistics and category tracking
- **🌐 Cross-Platform**: Windows n8n workflows + Ubuntu backend server
- **🔒 Secure Tunneling**: ngrok integration for secure remote access

## 🏗️ Architecture

- **Frontend/Workflow**: n8n automation workflows (Windows)
- **Backend API**: FastAPI server with YouTube integration (Ubuntu)
- **Tunneling**: ngrok for secure Windows ↔ Ubuntu communication
- **Media Server**: Jellyfin for music library management
- **Database**: SQLite for download tracking and analytics

## �� Quick Start

1. **Setup Backend** (Ubuntu):
   ```bash
   cd backend-python
   pip install -r requirements.txt
   export MUSIC_DIR=~/Media/music
   python enhanced_main.py
   ```

2. **Setup ngrok** (Ubuntu):
   ```bash
   ngrok http 5000
   ```

3. **Import n8n Workflow** (Windows):
   - Import `final-music-automation.json`
   - Configure YouTube API credentials
   - Update ngrok URL in workflow

4. **Configure Jellyfin**:
   - Set media library path to `~/Media/music`
   - Enable automatic library scanning

## 📁 Project Structure
