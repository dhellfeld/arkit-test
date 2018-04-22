# arkit-test
Learning to use ARKit to build augmented reality applications


* Steps to build and run arkit example with Macbook Pro 2016 (macOS 10.12) and iPhone 7 (iOS 11.3)
  - Latest Xcode version on Sierra (9.2) not compatible with iOS 11.3 (see issues below for fix)
  - Attached device to Macbook via lightning cable
  - Start Xcode, Select `Window`-->`Devices and Simulations` from top drop-down menu
  - Check "Show as run destination" and "Connect via network"
      - If on the same network, the lightning cable is no longer needed
  - If device setup hangs, click <kbd>+</kbd> from bottom left and go through setup manually
  - Create new project and select "Augmented Reality App"
  - Ensure the device is selected in top left
  - Three way to build and run:
      1. `Product`-->`Run`
      2. Press the $\blacktriangleright$ 
      3. <kbd>&#8984;B</kbd> then <kbd>&#8984;R</kbd>
  - Untrusted developer warning may appear on iPhone, navigate to `Settings`-->`General`-->`Profile & Device Management` and trust the developer
  - Team signing error can be solved by selecting a team under the signing section in the general tab of the project editor
  - Succesful build and run should open the arkit-test app on the iPhone and display a fighter jet in the camera scene (once camera access is granted)
      - Requires the iPhone to be unlocked
  - Three ways to close the app:
      1. `Product`-->`Stop`
      2. <kbd>&#8984;.</kbd>
      3. Close app on the iPhone

<!-- Issues -->
<details> <summary>Issues</summary>

- [x] Xcode 9.2 incompatible with iOS 11.3
    - Downloaded 11.3 device support from <https://github.com/filsv/iPhoneOSDeviceSupport/issues/7>
    - Unzip and rename `11.3`
    - Place in `/Applications/Xcode/Contents/Development/Platforms/iPhoneOS.platform/DeviceSupport/`
</details>
    
