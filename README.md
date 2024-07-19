

# Making OneUI faster and lighter

This repo is a list of things that can be disabled to make our device faster and lighter and by doing so, we can get more free RAM and more battery life. This list will be updated on a regular basis as more apps and more components will be tested if they are safe to disable.

Be sure to check the commits so you may see yourselves what stuffs were disabled for each update.

# Instructions

I recommend using Adhell which works even when unrooted. The advantage of using Adhell compared to using adb, especially when debloating, is that you don't need a computer plus, you can re-enable the apps without resetting your device.
Read the instructions for Adhell3 [here](https://github.com/pascua28/OneUI-Debloat/blob/master/Adhell3.md)

# Contributions

Feel free to open up any issues or even pull requests. I want to make this list as extensive as possible.

# Tests

I perform some tests after disabling every app/component to make sure it doesn't bring chaos to our devices. I've performed reboots after disabling them to ensure it doesn't cause bootloops and I ran logcat to make sure each app/component doesn't break another app/component.

# **OneUI Disabled Apps List**

This list is just a conservative debloat as even most bloat apps do not run in the background and a lot of bloat apps don't run as well when some of the features are disabled or not currently in use (like Smart Suggestions, Find My Mobile, Secure Folder, DeX, GPUWatch, etc). The goal of this is to disable as much apps while preserving more important features. Some apps were grouped together as they might be needed by other apps of the same group.

- Ad Services:
	- Ad Privacy (com.google.android.adservices.api)
	- com.google.android.ondevicepersonalization.services
	- Main Components (com.google.mainline.adservices)
- Android System Intelligence:
	- Android System Intelligence (com.google.android.as)
	- com.google.android.federatedcompute
	- com.google.android.overlay.gmsconfig.asi
	- Private Compute Services (com.google.android.as.oss)
- android.auto_generated_rro_product__
- AR Apps:
	- ARCore (com.google.ar.core) - A.K.A Play Services for AR
  - AR Doodle (com.samsung.android.ardrawing)
  - AR Emoji (com.samsung.android.aremoji)
  - AR Emoji Editor (com.samsung.android.aremojieditor)
  - AR Zone (com.samsung.android.arzone)
  - AutoDoodle (com.sec.android.autodoodle.service)
  - Crocro and friends (com.samsung.android.app.camera.sticker.facearavatar.preload)
 - AudioMirroring (com.samsung.android.audiomirroring)
- BBCAgent (com.samsung.android.bbc.bbcagent)
- Bixby vision:
  - Bixby Vision (com.samsung.android.visionintelligence)
  - BixbyVision Framework (com.samsung.android.bixbyvision.framework)
- Bixby voice:
  - Bixby Voice (com.samsung.android.bixby.agent)
  - SettingsBixby (com.samsung.android.app.settings.bixby)
  - Voice wake-up (com.samsung.android.bixby.wakeup)
- CCInfo (com.sec.android.CcInfo
- com.samsung.android.knox.attestation
- com.samsung.ucs.agen.ese
- Customization Service (com.samsung.android.rubin.app)
- Device Health Services (com.google.android.apps.turbo)
- Digital Wellbeing (com.samsung.android.forest)
- DQA (com.samsung.android.dqagent)
- Edge panels:
  - Apps (com.samsung.android.app.appsedge)
  - Clipboard edge (com.samsung.android.app.clipboardedge)
  - Edge panels (com.samsung.android.app.cocktailbarservice)
  - People (com.samsung.android.service.peoplestripe)
  - Tasks (com.samsung.android.app.taskedge)
  - Tools (com.sec.android.app.quicktool)
- Facebook bloats:
  - Meta App Installer (Facebook App Installer)
  - Meta App Manager (com.facebook.appmanager)
  - Meta Services (com.facebook.services)
- FACM (com.samsung.android.aircommandmanager) - Air gestures
- Galaxy apps:
  - App update (com.samsung.android.app.updatecenter)
  - Application recommendations (com.samsung.android.mapsagent)
  - Recommended apps (com.samsung.android.app.omcagent)
 - Galaxy Service Setup (com.samsung.android.dbsc)
 - Galaxy Themes (disable only if you don't have custom theme):
	 - Galaxy Themes (com.samsung.android.themestore)
	 - Galaxy Themes Services (com.samsung.android.themecenter)
- Gallery stories (com.samsung.storyservice) - Creates stories from your gallery
- Game Services:
  - Game Booster (com.samsung.android.game.gametools)
  - Game Launcher (com.samsung.android.game.gamehome)
  - Game Optimizing Service (com.samsung.android.game.gos)
- Google Bloatware:
  - Gmail (com.google.android.gm)
  - Google (com.google.android.googlequicksearchbox)
  - Google Assistant (com.android.hotwordenrollment.xgoogle)
  - Google Assistant (com.android.hotwordenrollment.okgoogle)
  - Google Location History (com.google.android.gms.location.history)
  - Google One Time Init (com.google.android.onetimeinitializer)
  - Google Partner Setup (com.google.android.partnersetup)
  - Google Safety Center Resources (com.google.android.safetycenter.resources)
  - Google Wi-Fi Provisioner (com.google.android.apps.carrier.carrierwifi)
  - Maps (com.google.android.apps.maps)
  - Meet (com.google.android.apps.tachyon)
  - Speech services by Google (com.google.android.tts)
  - YouTube (com.google.android.youtube)
 - HdmApp (com.samsung.android.hdmapp)
  - Hiya Service (com.hiya.star)
  - iaft (com.sec.android.iaft)
  - ImsLogger (com.sec.imslogger)
  - Knox Analytics Uploader (com.samsung.android.knox.analytics.uploader)
  - KnoxPushManager (com.samsung.android.knox.pushmanager)
  - KnoxZT Framework (com.samsung.android.knox.zt.framework) 
- Microsoft features:
  - Link to Windows Service (com.samsung.android.mdx)
  - OneDrive (com.microsoft.skydrive)
 - MobileWips (com.samsung.android.server.wifi.mobilewips)
 - NetworkDiagnostic (com.samsung.android.networkdiagnostic)
- Netflix (com.netflix.mediaclient)
- Peripheral Framework (com.samsung.android.peripheral.framework)
- Perso (com.sec.android.app.personalization)
- Phone (com.samsung.crane) - not the dialer app. This provides additional features to the Samsung dialer.
- Samsung Cloud:
	- Samsung Cloud (com.samsung.android.scloud)
	- Samsung Cloud Assistant (com.samsung.android.scpm)
- Samsung Free (com.samsung.android.app.spage)
- Samsung Pass:
  - Authentication Framework (com.samsung.android.authfw)
  - Autofill with Samsung Pass (com.samsung.android.samsungpassautofill)
  - Samsung Pass (com.samsung.android.samsungpass)
- Samsung Pay:
	- com.samsung.android.knox.mpos
  - Samsung PaymentFramework (com.samsung.android.spayfw)
  - Samsung Wallet_DKFW (com.samsung.android.carkey)
- Samsung Push Service (com.sec.spp.push) - Disabling this won't show you any prompts on your phone about new Samsung account logins on other devices.
- Samsung text-to-speech engine (com.samsung.SMT)
- Samsung Visit In (com.samsung.android.ipsgeofence)
- SecurityPolicy (com.samsung.aasaservice)
- Sharing apps:
  - Group Sharing (com.samsung.android.mobileservice)
  - Quick Share Agent (com.samsung.android.aware.service)
  - Quick Share (com.samsung.android.app.sharelive)
 - SilentLogging (com.sec.modem.settings)
- SIM Toolkit 1 (com.android.stk)
- SIM toolkit 2 (com.android.stk2)
- Smart Call (com.samsung.android.smartcallprovider)
- Smart Touch Call (com.samsung.android.visualars)
- SoHService (com.samsung.sait.sohservice)
- Software updates:
  - Software update (com.sec.android.soagent)
  - Software update (com.wssyncmldm)
- Sticker Center (com.samsung.android.stickercenter)
- Support components (com.google.mainline.telemetry)
- SVC Agent (com.samsung.android.svcagent)
- System Tracing (com.android.traceur)
- VolumeMonitorProvider (com.sec.android.app.volumemonitorprovider)
- WiFiAiService (com.samsung.android.wifi.ai)
- Wi-Fi tips (com.samsung.android.net.wifi.wifiguider)

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
