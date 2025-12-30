Windows Installation Instructions:
Method 1: Install using pip (Recommended)
bash
# Create a virtual environment (optional but recommended)
python -m venv venv
venv\Scripts\activate

# Install all requirements
pip install -r requirements.txt

# Or install individually
pip install Pillow piexif mutagen ffmpeg-python
Method 2: Install with FFmpeg for Windows
Download FFmpeg for Windows:

Go to: https://github.com/BtbN/FFmpeg-Builds/releases

Download ffmpeg-master-latest-win64-gpl.zip

Extract to C:\ffmpeg\

Add to PATH:

Press Win + X → System → Advanced system settings

Environment Variables → Path → Edit → Add C:\ffmpeg\bin

Install Python packages:

powershell
# Run PowerShell as Administrator
Set-ExecutionPolicy Bypass -Scope Process -Force

# Install Python packages
pip install Pillow piexif mutagen ffmpeg-python

# Verify installation
python -c "import PIL; import piexif; import mutagen; print('All dependencies installed successfully!')"
