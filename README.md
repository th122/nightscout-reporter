# Nightscout Reporter

A web app based on AngularDart to create PDF documents from nightscout data.

It retrieves CGM and treatment data stored in nightscout using the [API](https://github.com/nightscout/cgm-remote-monitor#nightscout-api) from
[cgm-remote-monitor](https://github.com/nightscout/cgm-remote-monitor) to create PDF reports.

## Local Installation
Nightscout Reporter needs [AngularDart](https://webdev.dartlang.org/angular).
After [installing dart](https://webdev.dartlang.org/guides/get-started#2-install-dart),
continue from the cloned nightscout-reporter directory to either build a html file to
run the application from, or start a web service to serve the code via localhost.

### Running from a file
* `pub get`
* `pub global activate webdev`
* `webdev build`    
* `pub upgrade`
*  now point the browser at the local starting file located at `build/index.html`

For some strange reason, Chromium works well on the remote nightscout-reporter site via http, but not on the local file.

### Served locally
[k2s described his approach](https://github.com/zreptil/nightscout-reporter/issues/21)

* `pub global activate webdev`
* `pub get`
* `webdev serve` to start a local server
* point your browser at `http://127.0.0.1:8080/`

Here Chrome/Chromium works fine, but not Firefox. 
