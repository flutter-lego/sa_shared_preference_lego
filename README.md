[![lego project](https://img.shields.io/badge/powered%20by-lego-blue?logo=github)](https://github.com/melodysdreamj/lego)
[![pub package](https://img.shields.io/pub/v/sa_shared_preference_lego.svg)](https://pub.dartlang.org/packages/sa_shared_preference_lego)

# sa_shared_preference_lego
Shared preference under [simple architecture lego framework](https://github.com/melodysdreamj/simple_architecture_lego).

##  Installation
1. open terminal in the lego project root directory, enter the following command for install cli.
   and create a new lego project if you don't have one.
```bash
flutter pub global activate lego_cli
lego create
```
2. in terminal, enter the following command for add lego to project.
```bash
lego add sa_shared_preference_lego
```

## Usage
```dart
Check check = await CheckSharedPreferences.get();
print(check.toMap());

check.s000 = "hello";

await CheckSharedPreferences.upsert(check);

Check check2 = await CheckSharedPreferences.get();
print(check2.toMap());
```
