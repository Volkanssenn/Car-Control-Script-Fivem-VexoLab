🚗 car-control (Advanced Vehicle iPad Interface)

Elevate your FiveM server's driving experience with car-control, an all-in-one, sleek iPad-style interface designed for QBCore. This script provides players with intuitive control over their vehicles, featuring a groundbreaking synchronized audio system.
✨ Key Features

    📱 Modern iPad Interface: A clean, responsive, and high-tech UI to manage your vehicle functions.

    🎶 Live Spatial Radio: The crown jewel of this script! Listen to live music and radio stations within your car. Thanks to advanced synchronization, people standing outside or near your vehicle can hear your music, making it perfect for car meets and street parties.

    💺 Dynamic Seat Shifting: Switch seats instantly with a click—no more getting out and back in to move to the passenger side.

    🚪 Door & Hood Control: Fully interact with every door, the trunk, and the hood of your vehicle through the digital interface.

    💾 Personal Playlists: Save your favorite tracks using the integrated database system.

🛠️ Installation Guide

Setting up car-control is straightforward. Follow these steps to get it running on your server:
1. Check Dependencies

Ensure you have the following resources installed and up-to-date:

    qb-core - Core Framework.

    oxmysql - For database operations (saving playlists).

    xsound - Critical for the spatial audio/music system.

2. Placement

    Download the script and place the car-control folder into your resources/[qb] directory.

    Note: Do not rename the folder. If you must change it, ensure you update the references in fxmanifest.lua.

3. Database Setup

    The script features an auto-install SQL system. Upon the first launch, it will automatically check for and create the player_playlists table if it doesn't exist. No manual SQL execution is required!

4. Server Configuration

Add the following to your server.cfg. Order is important; dependencies must start first:
Kod snippet'i

# Dependencies
ensure qb-core
ensure oxmysql
ensure xsound

# The Script
ensure car-control

5. Usage & Controls

    Open Interface: Press F4 while inside a vehicle.

    Customization: To change the default key, open client.lua and modify the key code on Line 6.

6. Verification

Once the server starts, check your console for these success messages:

    [iPad-V3] MySQL Global Wrapper: Stabilized and Active.

    [iPad-V3] INFO: Database table is verified.

⚠️ Troubleshooting

If you encounter issues with the music system, ensure that xsound is working correctly and is the latest version. The audio playback and spatial synchronization rely entirely on xsound logic.
