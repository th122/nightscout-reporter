# Nightscout Reporter

A web app based on AngularDart to create PDF documents from nightscout data.

It retrieves CGM and treatment data stored in nightscout using the [API](https://github.com/nightscout/cgm-remote-monitor#nightscout-api) from
[cgm-remote-monitor](https://github.com/nightscout/cgm-remote-monitor) to create PDF reports.

## Local Installation
There may be better procedures, but lacking any knowledge of dart or angular, this is how I proceeded:

Nightscout Reporter needs [AngularDart](https://webdev.dartlang.org/angular).
After [installing dart](https://webdev.dartlang.org/guides/get-started#2-install-dart), I continued from the nightscout-reporter directory:
* `pub get`
* `pub global activate webdev`
* `webdev build`    
* `pub upgrade`
*  now point the browser at the local starting file located at `build/index.html`

For some strange reason, Chromium works well on the remote nightscout-reporter site, but not on the local file.
