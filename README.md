# SC4 Performance Range 0.6

Trackman-style golf shot analysis UI for Android / Galaxy Z Fold series.

## Included
- Driving-range trajectory visualization (illustrative, not a measured 3D trajectory)
- SC4 manual shot entry: ball speed, launch angle/direction, carry, total, swing speed, spin, spin axis, apex, landing angle, hang time
- Smash factor calculation when swing speed is entered
- Shot history stored locally in browser WebView storage and CSV export
- Existing BLE scan/connect/GATT diagnostic shell from earlier prototype

## Important limitations
- SC4 automatic telemetry parsing is not implemented or verified against physical SC4 hardware.
- BLE connection/GATT discovery does not prove shot data is being received. SC4's actual characteristic UUIDs, notification payload format and decoding must be captured and validated.
- TrackMan club-delivery metrics such as club path, face angle, attack angle and dynamic loft are not fabricated. SC4 does not list these among its supported measurements.
- Flight curve and rendered trajectory are visual approximations; user-entered SC4 distances and values remain the source of truth.

## Build
Open this folder in Android Studio, sync Gradle, then Build > Build APK(s). Debug APK output is normally `app/build/outputs/apk/debug/app-debug.apk`.
