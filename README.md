# Gaitway Arcade

Games for Good — Spring 2025 Project

A collection of minigames set in an arcade, built in Unity with Wwise audio integration.

---

## Getting Started

### Prerequisites

- **Unity** — Make sure you're on the same editor version as the rest of the team. Open the project through Unity Hub and it will prompt you if you need to install the correct version.
- **Wwise** — The project uses Audiokinetic Wwise for audio. You'll need the [Wwise Launcher](https://www.audiokinetic.com/en/download) installed to open and modify Wwise projects. The Wwise Unity integration zips are included in the repo root (`WwiseUnityIntegration_Mac_Src.zip` and `WwiseUnityIntegration_Windows_Src.zip`). **NOTE: YOU WILL ONLY NEED WWISE IF YOU PLAN ON MODIFYING WWISE BASED AUDIO PROJECTS. IF YOU ARE USING UNITY AUDIO FOR YOUR GAME, IGNORE ALL WWISE RELATED LOGS, WARNINGS, AND ERRORS**
- **GitHub Desktop** — We use [GitHub Desktop](https://desktop.github.com/) for version control.

### Cloning the Repo

1. Open GitHub Desktop
2. Go to **File → Clone Repository**
3. Paste the URL: `https://github.com/hbjeletich/G4G-SP25.git`
4. Choose where you want it on your machine and click **Clone**

> **Video walkthrough:** The first half of [this video](https://youtu.be/8iG__tU92CE) covers how to use GitHub Desktop (cloning, pulling, pushing, etc.). The second half is specific to the Rhythm Kitchen game.

### Opening the Project

1. Open **Unity Hub**
2. Click **Open → Add project from disk**
3. Navigate to the folder you cloned and select it
4. Unity Hub will show the project — click to open it

---

## Captury Replay

### At-Home Testing

If you want to test your motion controls at home, you should use Captury Replay, which you can find here: [CapturyReplay](https://captury.com/resources/)

For Captury Replay, set your IP on your Tracking Area to 127.0.0.1. If you have GameSelect script in your scene, set that IP to 127.0.0.1 as well. 

Motion recordings for Replay can be found in this repo in the MotionRecordings folder. 

---

## Troubleshooting

### "No Git executable found" error in Unity

If you have GitHub Desktop installed but Unity (or another tool) throws an error saying it can't find `git`, it's because GitHub Desktop installs Git in a hidden location that isn't on your system PATH.

**Watch this quick fix video:** [No 'git' executable was found FIX!](https://www.youtube.com/watch?v=F-8A8mJwL_Y)

**The short version (Windows):**

1. Find where GitHub Desktop installed Git. It's usually at:
   ```
   C:\Users\<YourUsername>\AppData\Local\GitHubDesktop\app-<version>\resources\app\git\cmd\git.exe
   ```
2. Copy that path
3. Open **Start → search "Environment Variables" → Edit the system environment variables**
4. Under **System Variables**, find `Path` and click **Edit**
5. Click **New** and paste the Git path
6. Click **OK** on everything and restart Unity

---

## Project Structure

```
G4G-SP25/
├── Assets/                    # All Unity assets (scenes, scripts, prefabs, etc.)
├── Packages/                  # Unity package manifest
├── ProjectSettings/           # Unity project settings
├── G4G-SP25_WwiseProject/     # Main Wwise project
├── G4G-SP25-golfUpdate_WwiseProject/  # Golf game Wwise project
├── MotionRecordings/          # Motion capture recordings
└── README.md
```

---

## Useful Links

- **GitHub Desktop walkthrough + Rhythm Kitchen overview:** [https://youtu.be/8iG__tU92CE](https://youtu.be/8iG__tU92CE)
- **Git executable fix video:** [https://www.youtube.com/watch?v=F-8A8mJwL_Y](https://www.youtube.com/watch?v=F-8A8mJwL_Y)
