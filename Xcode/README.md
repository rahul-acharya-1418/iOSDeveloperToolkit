##### Clean Xcode caches

- Open Terminal `nano clean-xcode`
-  put below code
```
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
```
sudo xcrun simctl shutdown all
sudo xcrun simctl erase all
```
##### Create Python env
```
python3 -m venv path/to/venv
source path/to/venv/bin/activate
```
