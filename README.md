# numb-plugins
A repo containing all the community made plugins for Numb the calculator app.

In order to make a conversion plugin just a `.dart` and copy the template structure below.

```dart
Map<String, Map> lengthUnits = {
  'meter': {
    'id': 'm',
    'phrases': [
      'meters',
      'metre',
      'metres',
      'meter',
      'm',
      'meter',
      'meter',
      'meters',
      'meters'
    ],
    'unit': 1
  },
  'centimeter': {
    'id': 'cm',
    'phrases': [
      'centimeter',
      'centimeters',
      'centimetre',
      'cm',
      'centimetres',
      'cm'
    ],
    'unit': 0.01
  }
 }
```

make sure that the first object is your base value or S.I unit and the subsequent ones have a unit of 1 base unit in whatever the subsequent units might be.
**E.g:** 1 centimeter is equivalent to 0.01 meter. Therefore, 0.01 is the unit for centimeter
