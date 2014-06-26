## RubyOSINT v1

### Description
This is a simple ruby based tool used for OSINT/PenTesting an application. The first version has static URL entries that are commonly attacked (PHPMyAdmin, VPN, Email, Citrix, etc.

### Usage
```ruby OSINT.rb --url http(s)://xxx.xxx.xxx.xxx --uri list.txt```

### NEW USAGE
*bundle exec bin/osint https://TEST.com


### TODO
* Add CLI arguments
* add files to hold the URLs 
* Clean up the code
* Add target input via file
* Add scan output to file
* Add analysis of app headers to identify version of SharePoint and OWA.


### Known Issues

### Credits

* [@CarnalOwnage](https://twitter.com/carnal0wnage) for the ideas and some of the URL checks
* [Alex Levinson](https://twitter.com/alexlevinson) for helping with some ruby foo.
* [@alanjones](https://twitter.com/alanjones) for contributing and helping implement changes
### License
This code is licensed under the GPLv3. Full text of this can be found in ```LICENSE.txt```

### Changelog
* Added Color to the Command Line
* Added only reporting for 200 status (302 may be enabled by uncommenting it(be prepare for a lot of output).
* fixed the SSL invalid certs breaking to tool (alanjones)
* pulled the target URLs from the main .rb code and added to list.txt (alanjones)
* added ability to call options from CLI. (alanjones)
