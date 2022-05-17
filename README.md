# Every Door

The best mobile editor for adding shops and amenities to OpenStreetMap.

Help test it for [iOS](https://testflight.apple.com/join/5138nQCq) and
[Android](https://play.google.com/store/apps/details?id=info.zverev.ilya.every_door).

The roadmap is in [a project](https://github.com/users/Zverik/projects/1/views/2).

## Screenshots
<img src="https://wiki.openstreetmap.org/w/images/4/4c/Every_Door_0.3.0_Android_-_Main_Screen.png" width="170"/>
<img src="https://wiki.openstreetmap.org/w/images/f/f1/Every_Door_0.3.0_Android_-_Main_Screen_Aerial_View.png" width="170"/>
<img src="https://wiki.openstreetmap.org/w/images/a/af/Every_Door_0.3.0_Android_-_Add_Shop.png" width="170"/>
<img src="https://wiki.openstreetmap.org/w/images/4/42/Every_Door_0.3.0_Android_-_Edit_Screen.png" width="170"/>
<img src="https://wiki.openstreetmap.org/w/images/a/a3/Every_Door_0.3.0_Android_-_Main_Screen_Library.png" width="170"/>
<img src="https://wiki.openstreetmap.org/w/images/c/ce/Every_Door_0.3.0_Android_-_Edit_Tags_Screen.png" width="170"/>
<img src="https://wiki.openstreetmap.org/w/images/b/bc/Every_Door_0.3.0_Android_-_Mode_Addresses_Near_You.png" width="170"/>
<img src="https://wiki.openstreetmap.org/w/images/f/f7/Every_Door_0.3.0_Android_-_Mode_Features_Near_You.png" width="170"/>
<img src="https://wiki.openstreetmap.org/w/images/a/a5/Every_Door_0.3.0_Android_-_Configuration_Screen.png" width="170"/>
<a href="https://www.youtube.com/watch?v=oQao9KgC5f8"><img src="https://img.youtube.com/vi/oQao9KgC5f8/0.jpg" width="340"/></a>

## Presets and Translations

The editor uses [presets from iD](https://github.com/openstreetmap/id-tagging-schema):
they are managed in a dedicated repository and translated on Transifex.

Brands are managed in the [Name Suggestion Index](https://github.com/osmlab/name-suggestion-index).

For the time being Every Door localization is contained
[along the code](https://github.com/Zverik/every_door/tree/main/lib/l10n). You can either
make a new ARB file, or wait until I publish the translations to Weblate.

## Design

I need help with design. That includes [a new icon](https://github.com/Zverik/every_door/tree/main/icon),
[the website](https://github.com/Zverik/everydoor-website), Flutter animations for everything,
and general UX improvements. Please help.

## How To Build

1. Copy `lib/private.dart.sample` to `lib/private.dart` and put your OAuth and Bing keys there.
2. Download [taginfo-db.db](https://taginfo.openstreetmap.org/download) and unpack it somewhere (it's ~9 GB).
3. Run `tools/update.sh <path_to_taginfo_db>`.
4. `flutter pub get`.
5. `flutter run`.

## Author and License

The editor was written by © 2022 Ilya Zverev and published under the ISC license.
