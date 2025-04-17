QuranApp 📖

  
  
  
  


Overview
QuranApp is an Android application designed to help users read, explore, and understand the Al-Qur'an. It provides features like browsing Surah and Juz, bookmarking favorite ayat, and listening to audio recitations. The app also includes a settings page for a personalized experience, with support for Indonesian and English translations fetched from the Al-Qur'an API.
The app features a beautiful Islamic-themed background with a 9:16 aspect ratio, ensuring an immersive and visually appealing experience.
Features

Browse Surah and Juz: Explore the Al-Qur'an by Surah or Juz with detailed ayat views.
Ayat Translations: Supports Indonesian and English translations fetched from the Al-Qur'an API.
Audio Playback: Listen to ayat recitations with adjustable playback speed (0.5x to 2.0x) and auto-play option.
Bookmarking: Save your favorite ayat for quick access (feature coming soon).
Settings:
Toggle auto-play for audio recitations.
Adjust ayat text size (12sp to 24sp).
Switch between light and dark mode.
Choose translation language (Indonesian, English, or Arabic).
Enable/disable daily reading reminders using WorkManager.
Adjust audio playback speed.
Clear app cache to free up space.


Beautiful Design: Islamic-themed background with a purple hue, designed in a 9:16 aspect ratio for an immersive experience.
Navigation: Seamless navigation between Welcome, Menu, Surah Detail, Juz Detail, About Me, and Settings screens.

Tech Stack

Language: Java
Framework: Android SDK
Networking: Retrofit 2.9.0 (for fetching ayat data from Al-Qur'an API)
Database: Room (optional, for caching ayat data locally)
Background Tasks: WorkManager (for scheduling daily reminders)
UI: ConstraintLayout, RecyclerView, ViewPager
API: Al-Qur'an API (https://api.alquran.cloud)
Media: MediaPlayer (for audio playback)

Getting Started
Prerequisites

Android Studio (latest version recommended)
Android device/emulator running API 21 or higher
Internet connection (to fetch ayat data from the API)

Installation

Clone the repository:git clone https://github.com/yourusername/QuranApp.git


Open the project in Android Studio.
Sync the project with Gradle to download dependencies.
Add API permissions in AndroidManifest.xml:<uses-permission android:name="android.permission.INTERNET" />
<uses-permission android:name="android.permission.POST_NOTIFICATIONS" />


Run the app on an emulator or physical device.

Usage

Launch the app to see the WelcomeActivity with a beautiful Islamic background.
Navigate to the MenuActivity to choose between Surah, Juz, or Bookmarks.
Explore ayat in SurahDetailActivity or JuzDetailActivity, with options to view translations and play audio.
Customize your experience in the SettingsActivity:
Adjust text size, audio speed, or theme.
Choose your preferred translation language.
Enable daily reading reminders.


Visit the AboutMeActivity to learn more about the app and its creator.

Project Structure
QuranApp/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/quranapp/
│   │   │   │   ├── adapter/             # Adapters for RecyclerView (e.g., AyatAdapter, MenuSliderAdapter)
│   │   │   │   ├── api/                 # API-related classes (QuranApi, QuranService)
│   │   │   │   ├── model/               # Data models (Ayat, QuranResponse)
│   │   │   │   ├── WelcomeActivity.java # Entry point with navigation to other activities
│   │   │   │   ├── MenuActivity.java    # Main menu with slider for Surah, Juz, and Bookmarks
│   │   │   │   ├── SurahDetailActivity.java # Displays ayat for a specific Surah
│   │   │   │   ├── JuzDetailActivity.java   # Displays ayat for a specific Juz
│   │   │   │   ├── AboutMeActivity.java     # About page with app info
│   │   │   │   ├── SettingsActivity.java    # Settings page with customization options
│   │   │   │   ├── ReminderWorker.java      # WorkManager worker for daily reminders
│   │   │   ├── res/
│   │   │   │   ├── drawable/            # Images (e.g., bg_masjid.png, icons)
│   │   │   │   ├── layout/              # XML layouts for activities and adapters
│   │   │   │   ├── values/              # Strings, colors, and themes
│   │   │   ├── AndroidManifest.xml      # App manifest with permissions and activity declarations
│   ├── build.gradle                     # Module-level Gradle file with dependencies
├── build.gradle                         # Project-level Gradle file
├── README.md                            # This file

Contributing
Contributions are welcome! To contribute:

Fork the repository.
Create a new branch (git checkout -b feature/your-feature).
Make your changes and commit (git commit -m "Add your feature").
Push to your branch (git push origin feature/your-feature).
Create a pull request.

Please ensure your code follows the project's coding standards and includes appropriate tests.
License
This project is licensed under the MIT License - see the LICENSE file for details.
Acknowledgments

Al-Qur'an API for providing ayat data and translations.
Icons and images sourced from Android Studio's default resources.
Thanks to the Android developer community for their amazing libraries and tools.


Built with ☕ and passion by [Your Name].
