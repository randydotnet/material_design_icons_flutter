# material_design_icons_flutter

The [Material Design Icons](https://materialdesignicons.com/) Icon pack available as set of Flutter Icons.

Based on Material Design Icons 3.4.93.

## Installation

In the `dependencies:` section of your `pubspec.yaml`, add the following line:

```yaml
  material_design_icons_flutter: 3.1.3493
```

## Usage

```dart
import 'package:material_design_icons_flutter/material_design_icons_flutter.dart';

class MyWidget extends StatelessWidget {
  Widget build(BuildContext context) {
    return new IconButton(
      // Use the MdiIcons class for the IconData
      icon: new Icon(MdiIcons.sword), 
      onPressed: () { print('Using the sword'); }
     );
  }
}
```

Or, if you want to access the icon by a string name, instantiation a library of icons first.

```dart
import 'package:material_design_icons_flutter/material_design_icons_flutter.dart';

MdiIcons iconLib = new MdiIcons();

class MyWidget extends StatelessWidget {
  Widget build(BuildContext context) {
    return new IconButton(
      // Use the string name to access icons.
      icon: new Icon(iconLib['sword']), 
      onPressed: () { print('Using the sword'); }
     );
  }
}
```

## Name Conversion

Some icons' name is reversed keyword in Dart (and most other languages), so the names have been changed.

- `null` -> `nullIcon`
- `switch` -> `switchIcon`
- `sync` -> `syncIcon`
- `factory` -> `factoryIcon`
