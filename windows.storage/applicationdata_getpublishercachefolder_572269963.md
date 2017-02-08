---
-api-type: winrt method
---
 **Share files.** For example, if multiple apps use the same images or the same custom fonts, you can save these files in the shared storage folder.
 **Share the user's settings in a custom settings file.** For example, if multiple apps use temperatures, you can save a copy of the user's preference for Celsius or Fahrenheit in a custom settings file in the shared storage folder. We recommend that you also store the user's settings with each app or in another master location, however, since the user can clear the contents of the shared storage folder.
 Data in the shared storage folder is not backed up or roamed. Also, the user can clear the contents of the shared storage folder.
 You cannot use this feature to share data among apps from different publishers.
 You cannot use this feature to share data among different users.
 The shared storage folder does not have version management.
 There is no default subfolder. You have to specify a subfolder when you call the [GetPublisherCacheFolder](applicationdata_getpublishercachefolder.md) method.
 You can only access subfolders registered in the app manifest.
 You can't access the root of the shared storage folder.