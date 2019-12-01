# android-localization-helper
A python script that helps you create strings.xml for all languages in different hierarchical folder(using Google Translation API)

# usage

Syntax

```
python3.7 translator.py <source_lang_code> <string_file_name>
```

Eg,
```
python3.7 translator.py en strings.xml
```

Output will be created in transalted/ folder with various langugaes folders.

Paste them in your res/ folder of Android Project.

# credits

Combined effort from below repositories + Some Add Ons 

https://github.com/Ra-Na/GTranslate-strings-xml

https://github.com/Swisyn/android-strings.xml-translator


# other useful commands

Extract only strings from strings.xml
cut -d ">" -f2 strings.xml | cut -d "<" -f1

Extract non translatable strings from strings.xml
cat strings.xml|grep -v "translatable" | cut -d ">" -f2  | cut -d "<" -f1


