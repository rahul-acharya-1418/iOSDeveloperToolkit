##### Clean Xcode caches

- Open Terminal `nano clean-xcode`
- put below code
```bash
#!/bin/bash

rm -rf ~/Library/Developer/Xcode/UserData/Previews
rm -rf ~/Library/Developer/Xcode/DerivedData
rm -rf ~/Library/Developer/Xcode/Products
rm -rf ~/Library/Developer/Xcode/Archives
rm -rf ~/Library/Developer/Xcode/iOS\ DeviceSupport
```
- `chmod +x clean-xcode`
- `sudo mv /usr/local/bin/clean-xcode`
##### Reset All Simulators
```bash
sudo xcrun simctl shutdown all
sudo xcrun simctl erase all
```
##### Create Python env
```bash
python3 -m venv path/to/venv
source path/to/venv/bin/activate
```
##### Clean and Reinstall Pods
```bash
pod deintegrate
rm -rf Pods Podfile.lock StreamlyTV.xcworkspace
pod update
```
##### Add gitinto gitignore for remove
```bash
# macOS
.DS_Store
**/.DS_Store
```