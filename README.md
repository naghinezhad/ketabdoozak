## Setup and Dependencies

1. **Install Flutter SDK**

   - Ensure that you have the latest version of Flutter SDK installed on your system. You can download it from the official Flutter website:
     [https://flutter.dev/docs/get-started/install](https://flutter.dev/docs/get-started/install)

2. **Create or Enter a Flutter Project**

   - Open a terminal or command prompt and navigate to the directory where you want to create your Flutter project.
   - If you already have a project, navigate to its directory.

3. **Install Dependencies**

   - Run the following command to fetch and install the required dependencies:

     ```sh
     flutter pub get
     ```

   - This command reads the `pubspec.yaml` file and downloads all required packages and their transitive dependencies.

---

## Running the Application

### **Android**

1. Connect an Android device to your system or start an Android emulator.
2. Run the following command to build and launch the app on the Android device or emulator:

   ```sh
   flutter run android
   ```

### **iOS (Without Signing)**

1. Ensure that Xcode is installed on your macOS system.
2. To run the app on the iOS simulator, execute the following command:

   ```sh
   flutter run ios
   ```

   **Note:** This command runs the app on the simulator without signing. To deploy it on a physical iOS device, you need to set up code signing and provisioning profiles.

### **Web**

1. To run the web version of the app, execute the following command:

   ```sh
   flutter run web
   ```

   This will compile the Flutter app and launch it in a web browser.

---

## Building Release Versions

### **Android**

1. To build a final (release) APK for Android, run the following command:

   ```sh
   flutter build apk --release
   ```

   - The release APK will be located at:
     ```
     build/app/outputs/flutter-apk/app-release.apk
     ```

2. If you need an `App Bundle` for publishing on Google Play, use the following command:

   ```sh
   flutter build appbundle --release
   ```

   - The output will be located at:
     ```
     build/app/outputs/bundle/release/app-release.aab
     ```

### **iOS (Without Signing)**

1. To build an unsigned release version for iOS, run the following command:

   ```sh
   flutter build ios --release --no-codesign
   ```

   - The output will be located at:
     ```
     build/ios/ipa/app.ipa
     ```

### **Web**

1. To build a release version for the web, run the following command:

   ```sh
   flutter build web --release
   ```

   - The output files will be located at:
     ```
     build/web
     ```
   - These files can be deployed on a web server.

---

## Important Notes

- Ensure that you have the latest version of Flutter and all necessary dependencies installed.
- To run the application on iOS, you need a macOS system with Xcode installed.
- For the latest updates, refer to the official Flutter documentation: [https://flutter.dev/docs](https://flutter.dev/docs)
