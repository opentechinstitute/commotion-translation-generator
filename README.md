[![alt tag](http://img.shields.io/badge/maintainer-hawkinswnaf-blue.svg)](https://github.com/hawkinswnaf)

# commotion-translation-generator
=============================================

Parses commotion-router source files for user-facing strings and uses them to generate PO files for [https://github.com/opentechinstitute/luci-i18n-commotion](luci-i18n-commotion). The PO file generator will attempt to re-use any existing translations in the new PO file.

Translation of Commotion OpenWRT is managed on Transifex:
https://www.transifex.com/projects/p/commotion-user-interface/

## Prerequisites
* Perl 5
* perl modules (available through cpan)
  * DateTime
  * File::Copy
  * File::Next
  * File::Path
  * Git::Repository
  * Text::Balanced

## Usage

1. `$ cd scripts`
2. `$ ./parse.pl`

Newly generated PO files will be written to `scripts/working/translations/` and must be manually added to luci-i18n-commotion for upload to github.