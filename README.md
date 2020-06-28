# Text Field Problem when switching to Japanese Keyboard

0. Ensure you use Flutter Beta channel (1.19.0-4.2.pre, the up-to-date beta as of June 28th) and iOS
1. Open the app.
2. Ensure the keyboard is "English US".
3. Kill the app.
4. Open the app again.
5. Select the text field.
6. Change the keyboard to "日本語かな".
7. Type some Japanese characters such as "あいうえお".
8. You'll see the text field shows unexpected inputs such as "あああいあいあいうあいうあいうえあいうえ".


# Flutter Doctor

I use Flutter Beta channel for my iOS app.

```
~/Documents/beta_textfield_problem $ flutter doctor -v
[✓] Flutter (Channel beta, 1.19.0-4.2.pre, on Mac OS X 10.15.5 19F101, locale en-US)
    • Flutter version 1.19.0-4.2.pre at /Users/suztomo/development/flutter
    • Framework revision 9b9b543d92 (6 days ago), 2020-06-22 12:19:28 -0700
    • Engine revision 9a28c3bcf4
    • Dart version 2.9.0 (build 2.9.0-14.1.beta)

[✗] Android toolchain - develop for Android devices
    ✗ Unable to locate Android SDK.
      Install Android Studio from: https://developer.android.com/studio/index.html
      On first launch it will assist you in installing the Android SDK components.
      (or visit https://flutter.dev/docs/get-started/install/macos#android-setup for detailed instructions).
      If the Android SDK has been installed to a custom location, set ANDROID_SDK_ROOT to that location.
      You may also want to add it to your PATH environment variable.


 
[✓] Xcode - develop for iOS and macOS (Xcode 11.5)
    • Xcode at /Applications/Xcode.app/Contents/Developer
    • Xcode 11.5, Build version 11E608c
    • CocoaPods version 1.9.1

[!] Android Studio (not installed)
    • Android Studio not found; download from https://developer.android.com/studio/index.html
      (or visit https://flutter.dev/docs/get-started/install/macos#android-setup for detailed instructions).

[✓] IntelliJ IDEA Community Edition (version 2020.1.2)
    • IntelliJ at /Applications/IntelliJ IDEA CE.app
    • Flutter plugin version 46.0.3
    • Dart plugin version 201.7846.93

[✓] VS Code
    • VS Code at /Applications/Visual Studio Code.app/Contents
    • Flutter extension version 3.8.1

[✓] Connected device (1 available)
    • iPhone SE • f77bfc37802a5ad50f67ef7ae673b7fbea699e7b • ios • iOS 13.4.1

! Doctor found issues in 2 categories.
```