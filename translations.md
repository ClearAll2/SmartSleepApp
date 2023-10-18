# Smart Sleep Translations

This document details how you can contribute your translations for Smart Sleep.

## Structure

The [strings](https://github.com/ClearAll2/SmartSleepApp/tree/main/strings) folder contains all string values and is split into folders — one per language. These are named *values-X*, where *X* represents an [ISO 639-1 language code](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes). 

For example, *values-fr* represents the French language. Each folder houses a *strings.xml* file.

## How to translate

The *strings.xml* files house the copy displayed in Smart Sleep. They comprise an entry for each bit of text. For example:

```xml
<string name="privacy_text">Read our policy</string>
```

The `string` tags themselves must not be edited. To translate the above into French, you would use the folowing:

```xml
<string name="privacy_text">Lisez notre politique</string>
```

Some strings contain nested tags and/or placeholders:

```xml
<string name="to_sleep_now">If you sleep at %1$s:%2$s, you need to wake up at one of the following times:</string>
```

Placeholders (`%s` or `%1$s` or `%2$s`) tags must not be edited. To translate the above into French, you would use the folowing:

```xml
<string name="to_sleep_now">Si vous vous couchez à %1$s:%2$s, vous devez vous réveiller à l\'un des moments suivants :</string>
```

As such, a string of characters is translatable if preceded by `>` and suceeded by `<` or `<\`.

## Contributing

If a directory exists for your target language, edit the _strings.xml_ file inside. Otherwise, create a directory following the naming convention described in [Structure](#structure). Inside, copy and paste _strings.xml_ in [default values folder](https://github.com/ClearAll2/SmartSleepApp/tree/main/strings/values) and edit.

You are also welcome to correct existing translations. To do so, find the appropriate `string` tag in the localized _strings.xml_ file and edit its content. 

To submit a contribution for review, create a pull request. 

Thanks for your help!

© 2023 [LKONLE](mailto:lkonle@proton.me), and published to [Google Play Store](https://play.google.com/store/apps/details?id=com.lkonlesoft.smartsleep).
