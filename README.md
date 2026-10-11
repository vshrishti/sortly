🌷 About Sortly

Sortly is a lightweight file organization and automation tool built with Python. It helps keep your folders clean by automatically sorting files into categories based on their extensions.

Instead of manually organizing hundreds of files, Sortly does the repetitive work for you.

Whether it's documents, images, videos, audio files, archives, or code, Sortly makes file management simpler and more efficient.

✨ Features

📂 Automatic File Sorting — Organize files into categorized folders based on their extensions.

👀 Preview Mode — See planned file movements before making any changes.

🛡️ Safe File Handling — Avoid overwriting existing files by generating unique destination filenames.

📝 Activity Logging — Keep track of file movements and errors through log files.

⚡ Simple CLI — Run the organizer directly from your terminal.

🧩 Customizable Categories — Extend the file-extension mappings to suit your needs.

🛠️ Planned Features

🔍 Duplicate detection using SHA-256 hashing.

📊 CSV reports and organization statistics.

↩️ Undo and rollback functionality.

⏰ Scheduled file organization.

🖥️ An interactive Streamlit dashboard.

🧪 Automated testing with pytest.

🧰 Tech Stack

Technology

Purpose

Python 3.11+

Core application

pathlib

File and directory paths

shutil

Moving files

argparse

Command-line interface

logging

Activity and error logs

hashlib

Planned duplicate detection

pytest

Planned automated tests

Streamlit

Planned web dashboard

The current implementation uses Python's standard library, so no third-party packages are required.

📁 Project Structure

Sortly/
├── organizer.py
├── README.md
├── organizer.log
└── test_folder/
    ├── document.pdf
    ├── photo.jpg
    └── video.mp4

organizer.py — Main application.

README.md — Project documentation.

organizer.log — Generated activity log.

test_folder/ — Optional folder for testing.

🚀 Getting Started

1. Clone the repository

git clone https://github.com/YOUR_USERNAME/Sortly.git

2. Navigate to the project

cd Sortly

3. Check your Python version

python --version

Python 3.11 or newer is recommended.

4. Run Sortly

No additional dependencies are needed for the current version.

💻 Usage

Preview Mode

Preview how your files will be organized without moving anything:

python organizer.py "/path/to/your/folder"

Apply Changes

After reviewing the preview, organize the files:

python organizer.py "/path/to/your/folder" --apply

Windows example:

python organizer.py "C:\Users\YourName\Downloads"

Linux/macOS example:

python organizer.py "$HOME/Downloads"

Replace the example paths with the directory you want to organize.

Safety first: Always test Sortly on a temporary folder before using it on important files. The current version moves files when --apply is specified and does not yet support automatic rollback.

📦 Supported File Categories

Category

Extensions

📄 Documents

.pdf, .doc, .docx, .txt, .xlsx, .pptx

🖼️ Images

.png, .jpg, .jpeg, .gif, .webp

🎬 Videos

.mp4, .mkv, .mov, .avi

🎵 Audio

.mp3, .wav, .m4a

🗜️ Archives

.zip, .rar, .7z, .tar, .gz

💻 Code

.py, .js, .html, .css, .java, .cpp

📦 Others

All other extensions

🎯 Example

~ Before Sortly

Downloads/
├── resume.pdf
├── photo.jpg
├── tutorial.mp4
├── project.py
└── archive.zip

~ After Sortly

Downloads/
├── Documents/
│   └── resume.pdf
├── Images/
│   └── photo.jpg
├── Videos/
│   └── tutorial.mp4
├── Code/
│   └── project.py
└── Archives/
    └── archive.zip

📝 Logging

Sortly creates an organizer.log file to record successful file movements and errors.

These logs make it easier to troubleshoot problems and understand what happened during an organization run.

🗺️ Roadmap

Extension-based file categorization

Preview mode

Collision-safe filenames

Activity and error logging

Duplicate file detection

CSV report generation

Undo and rollback support

Scheduled automation

Streamlit dashboard

Automated tests

🔒 Safety & Limitations

Preview changes before applying them.

Test on sample folders before organizing important data.

Existing files are protected against filename collisions.

The current version does not include an undo feature.

The organizer processes files directly inside the selected folder, not files in nested subfolders.

Avoid organizing system directories or folders actively used by other applications.

🤝 Contributing

Contributions, suggestions, and improvements are welcome!

Fork this repository.

Create a feature branch.

Make your changes.

Test your implementation.

Submit a pull request with a clear description.

📄 License

This project is intended for learning, experimentation, and portfolio development.
this repository is published as MIT-licensed.

