
# Making OneUI faster and lighter

This repo is a list of things that can be disabled to make our device faster and lighter and by doing so, we can get more free RAM and more battery life. This list will be updated on a regular basis as more apps and more components will be tested if they are safe to disable.

Be sure to check the commits so you may see yourselves what stuffs were disabled for each update.

# Instructions

I recommend using Adhell which works even when unrooted. The advantage of using Adhell compared to using adb, especially when debloating, is that you don't need a computer plus, you can re-enable the apps without resetting your device. Installation instructions is here: https://forum.xda-developers.com/t/adhell-3-knox.3908002/post-85788393 and apk can be downloaded from here this repo.
The modified Adhell3 source can be found here: https://github.com/pascua28/adhell3

![alt text](https://github.com/pascua28/OneUI-Debloat/blob/master/Screenshots/1.jpg)
After installation make sure these toggles are enabled as shown.

After you have successfully installed Adhell, you can simply download adhell_backup.txt from this repo, place it to the folder that you created for Adhell, go to "Other->Settings" and select "Restore Database" and that's it. You may have to re-enable some apps or services depending on your needs.

You may also do it manually. If you want to disable apps, simply go to "Apps" tab, "Disable Apps" and toggle the apps you want to disable. If you want to disable app components manually, go to "Other", "Components" and select the app you want. After selecting the app, go to the respective components you want to disable (Services/Receivers/Providers). You may use this list as a guide regarding what things to disable.

![alt text](https://github.com/pascua28/OneUI-Debloat/blob/master/Screenshots/2.jpg)
Disable apps tab where you can enable/disable apps.

![alt text](https://github.com/pascua28/OneUI-Debloat/blob/master/Screenshots/3.jpg) ![alt text](https://github.com/pascua28/OneUI-Debloat/blob/master/Screenshots/4.jpg)
Components tab where you can enable/disable app permisions (below Android 12 only), activities, services, receivers and providers.

# Contributions

Feel free to open up any issues or even pull requests. I want to make this list as extensive as possible.

# Tests

I perform some tests after disabling every app/component to make sure it doesn't bring chaos to our devices. I've performed reboots after disabling them to ensure it doesn't cause bootloops and I ran logcat to make sure each app/component doesn't break another app/component.

# **OneUI Disabled Apps List**

This list is just a conservative debloat. The goal of this is to disable as much apps while preserving more important features. Some apps were grouped together as they might be needed by other apps of the same group.

- 3 Button Navigation Bar (com.android.internal.systemui.navbar.threebutton)
- AASAservice (com.samsung.aasaservice)
- Adapt Sound (com.sec.hearingadjust)
- Android Auto (com.google.android.projection.gearhead) - Use apps on your vehicle
- Android S Easter Egg (com.android.egg)
- Android system intelligence and Private Compute Services (com.google.android.as, com.google.android.as ) - Needed by adaptive battery
- AR Apps:
  - AR Doodle (com.samsung.android.ardrawing)
  - AR Emoji (com.samsung.android.aremoji)
  - AR Zone (com.samsung.android.arzone)
  - AutoDoodle (com.sec.android.autodoodle.service)
  - Crocro and friends (com.samsung.android.app.camera.sticker.facearavatar.preload)
- ARCore (com.google.ar.core) - A.K.A Play Services for AR
- Auto Hotspot (com.sec.mhs.smarttethering)
- Bixby vision:
  - Bixby Vision (com.samsung.android.visionintelligence)
  - BixbyVision Framework (com.samsung.android.bixbyvision.framework)
- Bixby voice:
  - Bixby dictation (com.samsung.android.bixby.service)
  - Bixby Voice (com.samsung.android.bixby.agent)
  - SettingsBixby (com.samsung.android.app.settings.bixby)
  - SystemUIBixby2 (com.samsung.systemui.bixby2)
  - Voice wake-up (com.samsung.android.bixby.wakeup)
- BluetoothTest (com.sec.android.app.bluetoothtest)
- Call & text on other devices (com.samsung.android.mdecservice)
- Camera services (these stuffs doesn't seem to provide any additional functionality)
  - Cameralyzer (com.sec.factory.cameralyzer)
  - FactoryCamera (com.sec.factory.camera)
  - SCameraService (com.samsung.android.camerasdkservice)
  - SCameraXService (com.samsung.android.cameraxservice)
- Cell Broadcast Service (com.google.android.cellbroadcastservice) - needed to receive broadcast messages
- ChromeCustomizations (com.sec.android.app.chromecustomizations)
- ClipboardSaveService (com.samsung.clipboardsaveservice)
- Customization Service (com.samsung.android.rubin.app)
- DECO PIC (com.samsung.android.livestickers)
- Device Health Services (com.google.android.apps.turbo)
- Device security (com.samsung.android.sm.devicesecurity) - Device protection found under device care
- Device Test (com.sec.factory)
- Dictionary (com.diotek.sec.lookup.dictionary)
- Digital Wellbeing (com.samsung.android.forest)
- Dual Messenger (com.samsung.android.da.daagent)
- Edge panels:
  - Apps (com.samsung.android.app.appsedge)
  - Clipboard edge (com.samsung.android.app.clipboardedge)
  - Edge panels (com.samsung.android.app.cocktailbarservice)
  - People (com.samsung.android.service.peoplestripe)
  - Tasks (com.samsung.android.app.taskedge)
  - Tools (com.sec.android.app.quicktool)
- Error (com.sec.app.RilErrorNotifier)
- Facebook bloats:
  - Meta App Installer (Facebook App Installer)
  - Meta App Manager (com.facebook.appmanager)
  - Meta Services (com.facebook.services)
- FaceService (com.samsung.faceservice) - No idea what this is but face unlock still works without it
- FACM (com.samsung.android.aircommandmanager) - Air gestures
- Find My Mobile (com.samsung.android.fmm)
- Galaxy apps:
  - App update (com.samsung.android.app.updatecenter)
  - Application recommendations (com.samsung.android.mapsagent)
  - Recommended apps (com.samsung.android.app.omcagent)
- Galaxy Themes (com.samsung.android.themestore)
- Gallery stories (com.samsung.storyservice) - Creates stories from your gallery
- Game Services:
  - Game Booster (com.samsung.android.game.gametools)
  - Game Launcher (com.samsung.android.game.gamehome)
  - Game Optimizing Service (com.samsung.android.game.gos)
- Google Bloatware:
  - Duo Installer (com.google.android.apps.tachyon) - Installs Google Duo annoyingly
  - Gmail (com.google.android.gm)
  - Google (com.google.android.googlequicksearchbox)
  - Google Assistant (com.android.hotwordenrollment.xgoogle)
  - Google Assistant (com.android.hotwordenrollment.okgoogle)
  - Google Location History (com.google.android.gms.location.history)
  - Google One Time Init (com.google.android.onetimeinitializer)
  - Google Partner Setup (com.google.android.partnersetup)
  - Google Wi-Fi Provisioner (com.google.android.apps.carrier.carrierwifi)
  - Maps (com.google.android.apps.maps)
  - Speech services by Google (com.google.android.tts)
  - YouTube (com.google.android.youtube)
- GPUWatch (com.samsung.gpuwatchapp)
- HandwritingService (com.samsung.android.sdk.handwriting)
- Live Transcribe & Sound Notifications (com.google.audio.hearing.visualization.accessibility.scribe)
- Live Wallpaper Picker (com.android.wallpaper.livepicker)
- Magnifier (com.sec.android.app.magnifier)
- Market Feedback Agent (com.google.android.feedback)
- Media and devices (com.samsung.android.mdx.quickboard)
- Microsoft features:
  - Link to Windows Service (com.samsung.android.mdx)
  - OneDrive (com.microsoft.skydrive)
 - Modes and Routines (com.samsung.android.app.routines)
- Nearby devices apps:
  - Nearby device scanning (com.samsung.android.easysetup)
  - Nearby device scanning (com.samsung.android.beaconmanager)
  - Nearby Service (com.samsung.android.allshare.service.mediashare)
  - Your Phone Companion (com.microsoft.appmanager)
- Netflix (com.netflix.mediaclient)
- NFC (com.android.nfc)
- Noto Serif / Source Sans Pro (com.android.theme.font.notoserifsource) - Just a font
- NSDSWebApp (com.sec.vsim.ericssonnsds.webapp)
- PartnerNetflixActivation (com.netflix.partner.activation)
- Samsung ApexService (com.sec.android.app.apex)
- Samung DeX:
  - DeX for PC (com.sec.android.app.dexonpc)
  - Samsung DeX (com.sec.android.desktopmode.uiservice)
  - Samsung DeX home (com.sec.android.app.desktoplauncher)
  - Samsung DeX System UI (com.samsung.desktopsystemui)
- Samsung Free (com.samsung.android.app.spage)
- Samsung Galaxy Friends (com.samsung.android.mateagent)
- Samsung Location SDK (com.sec.location.nsflp2)
- Samsung Pass:
  - Authentication Framework (com.samsung.android.authfw)
  - AuthFw TaPack (com.samsung.android.tapack.authfw)
  - Autofill with Samsung Pass (com.samsung.android.samsungpassautofill)
  - Samsung Pass (com.samsung.android.samsungpass)
  - Samsung Pass (com.samsung.android.dkey)
- Samsung Pay:
  - Samsung PaymentFramework (com.samsung.android.spayfw)
  - Samsung Wallet_DKFW (com.samsung.android.carkey)
- Samsung Push Service (com.sec.spp.push)
- Samsung Setup Wizard (com.sec.android.app.SecSetupWizard)
- Samsung text-to-speech engine (com.samsung.SMT)
- Samsung Visit In (com.samsung.android.ipsgeofence)
- Samsung voice input (com.samsung.android.svoiceime)
- SamsungOne (com.monotype.android.font.samsungone) - Just a font
- SetupWizardLegalProvider (com.sec.android.app.setupwizardlegalprovider)
- Sharing apps:
  - Group Sharing (com.samsung.android.mobileservice)
  - Quick Share (com.samsung.android.aware.service)
  - Quick Share (com.samsung.android.app.sharelive)
- SIM Toolkit 1 (com.android.stk)
- SIM toolkit 2 (com.android.stk2)
- Smart suggestions (com.samsung.android.smartsuggestions)
- Smart Touch Call (com.samsung.android.visualars)
- Smart View (com.samsung.android.smartmirroring)
- SmartFaceService (com.samsung.android.smartface) - Smart stay
- SmartThings Framework (com.samsung.android.service.stplatform)
- Software updates:
  - Software update (com.sec.android.soagent)
  - Software update (com.wssyncmldm)
  - SystemUpdate (com.sec.android.systemupdate)
- Sticker Center (com.samsung.android.stickercenter)
- Support components (com.google.mainline.telemetry) - Related to telemetry and data collection
- Tags (com.samsung.android.service.tagservice)
- TalkBack (com.samsung.android.accessibility.talkback) - An accessibility service that reads texts aloud
- TetheringAutomation (com.sec.automation)
- User Dictionary (com.android.providers.userdictionary)
- Video call effects (com.samsung.android.vtcamerasettings)
- VolumeMonitorProvider (com.sec.android.app.volumemonitorprovider)
- Wallpaper services (com.samsung.android.dynamiclock)
- Weather (com.sec.android.daemonapp)
- Wi-Fi Calling (com.sec.unifiedwfc)
- Wi-Fi tips (com.samsung.android.net.wifi.wifiguider)
- Wireless emergency alerts (com.google.android.cellbroadcastreceiver)
- WlanTest (com.sec.android.app.wlantest)
- Work profile:
  - Work profile (com.samsung.android.knox.containercore)
  - Work Setup (com.android.managedprovisioning)

# Google Play Services Disabled Components List

You may want to clear Google Play Services app data after disabling any of these.

## If you don't want to search and disable every service, provider or receiver, you can just disable all of Google Play Services receivers.
## Providers:

- ReportingContentProvider (com.google.android.location.reporting.service.utils.ReportingContentProvider)
- FastPairContextualCardProvider (com.google.android.gms.nearby.discovery.fastpair.slice.FastPairContextualCardProvider)
- FastPairSliceProvider (com.google.android.gms.nearby.discovery.fastpair.slice.FastPairSliceProvider)
- SharingSliceProvider (com.google.android.gms.nearby.sharing.SharingSliceProvider)

### Receivers:

- Ad-related receivers:
  - FlagsReceiver (com.google.android.gms.ads.config.FlagsReceiver)

- Analytics and reporting services:

  - AnalyticsReceiver (com.google.android.gms.analytics.AnalyticsReceiver)
  - UsageReportingIntentService (com.google.android.gms.usagereporting.service.UsageReportingIntentService)

- App measurement receivers:

  - AppMeasurementReceiver (com.google.android.gms.measurement.AppMeasurementReceiver)

  - AppMeasurementReceiver (com.google.android.gms.measurement.PackageMeasurementReceiver)

### Services:

- Ad-related services:
  - AdRequestBrokerService (com.google.android.gms.ads.AdRequestBrokerService)
  - CacheBrokerService (com.google.android.gms.ads.cache.CacheBrokerService)
  - AdvertisingIdNotificationService (com.google.android.gms.ads.identifier.service.AdvertisingIdNotificationService)
  - AdvertisingIdService (com.google.android.gms.ads.identifier.service.AdvertisingIdService)
  - NegotiationService (com.google.android.gms.ads.jams.NegotiationService)
  - GmpConversionTrackingBrokerService (com.google.android.gms.ads.measurement.GmpConversionTrackingBrokerService)
  - GcmSchedulerWakeupService (com.google.android.gms.ads.social.GcmSchedulerWakeupService)

- Analytics and reporting services:

  - AnalyticsService (com.google.android.gms.analytics.AnalyticsService)

  - AnalyticsTaskService (com.google.android.gms.analytics.AnalyticsTaskService)

  - PlayLogReportingService (com.google.android.gms.analytics.internal.PlayLogReportingService)

  - AnalyticsService (com.google.android.gms.analytics.service.AnalyticsService)

- App measurement services:

  - AppMeasurementJobService (com.google.android.gms.measurement.AppMeasurementJobService)
  - AppMeasurementService (com.google.android.gms.measurement.AppMeasurementService)
  - PackageMeasurementService (com.google.android.gms.measurement.PackageMeasurementService)
  - PackageMeasurementTaskService (com.google.android.gms.measurement.PackageMeasurementTaskService)
  - MeasurementBrokerService (com.google.android.gms.measurement.service.MeasurementBrokerService)

- Context manager services (probably used for data collection):

  - ContextManagerService (com.google.android.contextmanager.service.ContextManagerService)
  - ContextManagerTaskService (com.google.android.contextmanager.sync.ContextManagerTaskService)

- Location services:

  - Leave these services enabled if you use location history and sharing
    - LocationHistoryInjectorService (com.google.android.location.reporting.service.LocationHistoryInjectorService)
    - LocationSharingSettingInjectorService (com.google.android.gms.locationsharing.service.LocationSharingSettingInjectorService)
    - LocationSharingService (com.google.android.gms.locationsharing.service.LocationSharingService)
  - LocationAccuracyInjectorService (com.google.android.location.util.LocationAccuracyInjectorService)
  - LocationPersistentService (com.google.android.gms.location.persistent.LocationPersistentService)
  - PlacesTaskService (com.google.android.location.places.PlacesTaskService)
  - PlaceDetectionAsyncService (com.google.android.location.places.service.PlaceDetectionAsyncService)
  - PeriodicReporterMonitoringService (com.google.android.gms.locationsharingreporter.service.reporting.periodic.PeriodicReporterMonitoringService)
  - DispatchingService (com.google.android.location.reporting.service.DispatchingService)
  - ReportingAndroidService (com.google.android.location.reporting.service.ReportingAndroidService)
  - ReportingSyncService (com.google.android.location.reporting.service.ReportingSyncService)
  - UploadGcmTaskService (com.google.android.location.reporting.service.UploadGcmTaskService)
  - GeocodeService (com.google.android.gms.location.geocode.GeocodeService)
  - GcmReceiverService (com.google.android.gms.location.quake.ealert.GcmReceiverService)
  - These 2 services can be safely disabled but breaks some location functionalities. Google Maps still works with these 2 disabled but the camera app needs these 2 if you want to add location tags to your photos
    - GoogleLocationService (com.google.android.location.internal.server.GoogleLocationService)
    - GoogleLocationManagerService (com.google.android.location.internal.GoogleLocationManagerService)

- Media cast-related services:

  - CastMediaRoute2ProviderService (com.google.android.gms.cast.media.CastMediaRoute2ProviderService)
  - CastRemoteDisplayProviderService (com.google.android.gms.cast.media.CastRemoteDisplayProviderService)
  - CastPersistentService (com.google.android.gms.cast.service.CastPersistentService)
  - CastSocketMultiplexerLifeCycleService (com.google.android.gms.cast.service.CastSocketMultiplexerLifeCycleService)

- Nearby connection services:

  - NearbyConnectionsAndroidService (com.google.android.gms.nearby.connection.service.NearbyConnectionsAndroidService)
  - DiscoveryService (com.google.android.gms.nearby.discovery.service.DiscoveryService)
  - WakeUpService (com.google.android.gms.nearby.exposurenotification.WakeUpService)
  - ExposureMatchingService (com.google.android.gms.nearby.exposurenotification.service.ExposureMatchingService)
  - ExposureMatchingTriggerService (com.google.android.gms.nearby.exposurenotification.service.ExposureMatchingTriggerService)
  - ExposureNotificationInternalService (com.google.android.gms.nearby.exposurenotification.service.ExposureNotificationInternalService)
  - NfcAdvertisingService (com.google.android.gms.nearby.mediums.nearfieldcommunication.NfcAdvertisingService)
  - DebugPokeService (com.google.android.gms.nearby.messages.debug.DebugPokeService)
  - OfflineCachingService (com.google.android.gms.nearby.messages.offline.OfflineCachingService)
  - NearbyMessagesService (com.google.android.gms.nearby.messages.service.NearbyMessagesService)
  - DirectShareService (com.google.android.gms.nearby.sharing.DirectShareService)
  - ReceiveSurfaceService (com.google.android.gms.nearby.sharing.ReceiveSurfaceService)
  - SharingSyncService (com.google.android.gms.nearby.sharing.SharingSyncService()
  - SharingTileService (com.google.android.gms.nearby.sharing.SharingTileService)
  - NearbyDirectService (com.google.location.nearby.direct.service.NearbyDirectService)

- Task scheduling services (not sure what these are):

  - TaskExecutionService (com.google.android.gms.gcm.nts.TaskExecutionService)
