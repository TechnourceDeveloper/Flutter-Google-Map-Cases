
# Google Map Module

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:


    - [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)  
    - [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)  


For help getting started with Flutter development, view the  
[online documentation](https://docs.flutter.dev/), which offers tutorials,  
samples, guidance on mobile development, and a full API reference.


Softwares and Version Install Flutter (3.10.1) :

https://docs.flutter.dev/get-started/install    
Install Android Studio : Android Studio Dolphin | 2021.3.1 Patch 1

https://developer.android.com/studio/install    
Xcode (14.2) Install :

https://apps.apple.com/us/app/xcode/id497799835?mt=12

# Features :

- Select and search location with marker at location
- Drag marker to get address of that location
- Multiple and custom markers at map
- Route draw between two points
- Cluster on google map

# Clone Project :

git clone https://github.com/TechnourceDeveloper/Flutter-Google-Map-Cases.git

Steps after project clone successfully.
1. Enable dart support to the current project.
2. If configuration not set then in android studio go to add configuration and add path of main.dart
3. Go to pubspec.yaml file or into terminal of project path run command: flutter pub get
4. After these steps run project.

# About Project files:

State Management Pattern used Getx Pattern (get: ^4.6.5)

https://pub.dev/packages/get    
All global and constants are declared in global folder

**PUT YOUR GOOGLE PLACES API KEY HERE TO MAKE IT WORK**
**path: lib/global/utils/config.dart**
**kGoogleApiKey** is defined in config file.

class Config {  
static var appName = "Google Map Module";  
***static var kGoogleApiKey = 'PUT_YOUR_API_KEY_HERE';***

lib/global/utils/config.dart

# This app contains 4 buttons.

# 1. Search Location
- Search location Google Map will load, and the user's current location and address will be displayed in Google Map.
- Users can also drag marker to get a particular place's address.
- Users can search for any place by using the autocomplete search box, and a marker will move to that location.

**Used Plugins:**

- To load Google Map we use this package:  
  google_maps_flutter - https://pub.dev/packages/google_maps_flutter
- To get the current location and address, we use this packages:
1. geolocator - https://pub.dev/packages/geolocator
2. geocoding - https://pub.dev/packages/geocoding
- To get autocomplete place search box we use Google Places API.

**Screenshots:**

![1](https://github.com/TechnourceDeveloper/Flutter-Google-Map-Cases/assets/70566076/328a557d-3f13-4ff5-821f-0702335074a2)
![2](https://github.com/TechnourceDeveloper/Flutter-Google-Map-Cases/assets/70566076/13d2bb69-aab0-43eb-a334-9dc5cb7c8259)
![3](https://github.com/TechnourceDeveloper/Flutter-Google-Map-Cases/assets/70566076/499eda70-b6fa-4684-9b48-7ee62a83a8bc)
![4](https://github.com/TechnourceDeveloper/Flutter-Google-Map-Cases/assets/70566076/dc3944b1-ebb8-4c1b-a2a4-1b00327f3f1b)
![5](https://github.com/TechnourceDeveloper/Flutter-Google-Map-Cases/assets/70566076/8981631e-774d-4632-b42b-4a314f0b20aa)




# 2. Multiple Custom Marker
- On click of multiple marker users will find places like restaurants, hospitals, banks, etc. marked.
- Users can also select a custom marker and replace it with the default marker.

**Used Plugins:**

- To get Near by places, we use this package:  
  google_maps_webservice - https://pub.dev/packages/google_maps_webservice

**Screenshots:**

![6](https://github.com/TechnourceDeveloper/Flutter-Google-Map-Cases/assets/70566076/9e103521-96ac-4af0-af8b-845b585402e6)
![7](https://github.com/TechnourceDeveloper/Flutter-Google-Map-Cases/assets/70566076/b43e92fc-53e4-4220-90da-2a322da1d00e)

# 3. Route Draw
- On click of route draw Users current location will be display in google map.
- A user can search for his destination and see the route from his sources to the destination.

**Used Plugins:**

- To show route we use this package:  
  flutter_polyline_points  - https://pub.dev/packages/flutter_polyline_points

**Screenshots:**

![8](https://github.com/TechnourceDeveloper/Flutter-Google-Map-Cases/assets/70566076/d3f29c14-f895-4152-b91a-00c75b85ca19)
![9](https://github.com/TechnourceDeveloper/Flutter-Google-Map-Cases/assets/70566076/d9f09e7f-db9f-43c4-86a9-72f482cf056a)

# 4. Cluster
- On click of cluster **The number on a cluster indicates how many markers it contains**. As you zoom into any of the cluster locations, the number on the cluster decreases, and you begin to see the individual markers on the map. Zooming out of the map consolidates the markers into clusters again.

**Used Plugins:**
- For cluster, we use this package:  
  google_maps_cluster_manager -  https://pub.dev/packages/google_maps_cluster_manager

**Screenshots:**

![10](https://github.com/TechnourceDeveloper/Flutter-Google-Map-Cases/assets/70566076/4cadbf5e-218a-4881-9336-8d9291ac4fc7)


## License

[MIT](LICENSE)
