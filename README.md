# Simple Location Tracker App

## App Description
This mobile application is designed to track and display the user's real-time location on a map. By integrating Android Location Services with the Google Maps SDK, the app retrieves the device's current coordinates (latitude and longitude). A blue marker on the map represents the user, and this marker updates automatically as the device moves, providing a live visualization of the user's position.

## Permissions Used
To function correctly, the app requests the following permissions in the `AndroidManifest.xml` file:
* **ACCESS_FINE_LOCATION:** This allows the app to access the precise location of the device using GPS.
* **ACCESS_COARSE_LOCATION:** This allows the app to access the approximate location using network sources (Wi-Fi and cell towers).
* **INTERNET:** This is required to download map data and tiles from Google servers.

## How GPS Location is Obtained
The Global Positioning System (GPS) works by communicating with satellites orbiting the Earth. The device receives signals from these satellites to calculate its exact position. In this app, we use the Android Location API to request this data. Once the user grants permission, the app listens for location updates and passes the coordinate data (latitude and longitude) to the Google Map, which then renders the blue "My Location" dot at the correct spot on the screen.

## Screenshots of the Running App
| Permission Request | Map Display | Location Update |
|:------------------:|:-----------:|:---------------:|
| ![Permission Request](screenshots/permission_request.png) | ![Map Display](screenshots/map_location.png) | ![Location Update](screenshots/location_update.png) |
