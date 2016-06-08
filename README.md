# libloader
------

For load all library located at folder 'libloader' on sideloaded Apps
* Can be used too for force library to load on Apps Thats Is Protected for Jailbreak Check's (like bank's client and other apps)

How to use
------

* Rename App file extension .ipa to .zip and Extract
* Open main App Executable(like: Payload/AppName.app/AppName) on any Hex Editor
* Replece all occurencies of string "/usr/lib/libSystem.B.dylib" to "@executable_path/Sys.dylib" and Save Changes
* Copy file Sys.dylib to same Dir of App Executable(like: Payload/AppName.app/)
* Create folder "libloader" on same Dir of App Executable(like: Payload/AppName.app/) and copy any library .dylib thats you want to load
Structure like this:
    /Payload/
    	/AppName.app/
			AppName
			Info.plist
			Sys.dylib
			/libloader/
				myTweaked.dylib
				myLibrary.dylib
				anotherPatcher.dylib
				myHack.dylib
* Compress back to zip and rename compressed file extension .zip to .ipa
* Use [iOS App Signer](https://dantheman827.github.io/ios-app-signer/) to sign and install with iTunes/Xcode/other.

