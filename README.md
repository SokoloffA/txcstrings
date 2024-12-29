# txcstrings
Scripts for localization of swift and objective-C programs via transifex.com

Apple recommends using string catalog (.xcstrings files) to localize applications. The scripts in this project allow you to integrate .xcstrings files with transifex.com.

## Instalation
1. [Localize texts in your application](https://developer.apple.com/documentation/xcode/localizing-and-varying-text-with-a-string-catalog).
2. [Add a string catalog to your project](https://developer.apple.com/documentation/xcode/localizing-and-varying-text-with-a-string-catalog).
3. Do not add languages to your project.
4. [Create a project on transifex.com](https://help.transifex.com/en/articles/6236785-creating-a-project).
5. Copy the contents of the tx directory from this project to the **.tx** directory of your project. *Note that the directory name must start with a dot.*
6. [Create a .tx/config file, you can use the tx/config.example file as an example](https://help.transifex.com/en/articles/6236785-creating-a-project).

## Using
1. Use the .tx/upload.py script to update the source strings on transifex.com.
1. Use the .tx/download.py script to download translations to your project. If there is a new language, it will be automatically added to your xcode project.
