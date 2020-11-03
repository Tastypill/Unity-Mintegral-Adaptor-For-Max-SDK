# Unity-Mintegral-Adaptor-For-Max-SDK

Mintegral Adapter for AppLovin Max Unity SDK : 

1. Make sure you removed Mintegral Adapter completely from unity project. To do this, delete Assets -> MaxSdk -> Mediation -> Mintegral folder.

2. Import "max-mintegrak-adapter-android-14.6.2-iOS-6.6.x.unitypackage" to project. 

3. No additional steps required for android.

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Additional steps to update Mintegral SDK to latest version for iOS : 

1. Build Unity Project and Generate Xcode project as normal process.
2. Locate Xcode Project and Open PodFile.
3. Remove  [ pod 'AppLovinMediationMintegralAdapter', '6.4.1.0.1' ] from PodFile and save.
4. Open Terminal at Xcode project Folder Location.
5. Run Below Pod commands.
	A. pod Install
	B. pod cache clean 'MintegralAdSDK' --all
6. Open PodFile Again.
7. Add [ pod 'AppLovinMediationMintegralAdapter', '6.4.1.0.1' ] back again and save file.
8. Open Terminal at Xcode project Folder Location.
9. Run Below Pod commands.
	A. Pod Install
10. Mintegral SDK should be updated to latest version.

* This needs to be perform only once.


