Odometer
========

Odometer is a Javascript and CSS library for smoothly transitioning numbers.

Fork of https://github.com/HubSpot/odometer with patches that fix longstanding issues. Our forked version allows leading or trailing zeros to be configured in the constructor options:

For leading zeros, use minIntegerLen. For trailing zeroes, create the format string with capital 'D', e.g. "(,ddd).DD".

Example Usage:
```
var odometer = new Odometer({
    minIntegerLen: 4,
    format: 'ddd.DD',
    value: 1.2
});

$scope.$watch("foo", function(newVal) {
    odometer.update(newVal);
});

//odometer would read "0001.20" initially
```
### [Overview](http://github.hubspot.com/odometer/docs/welcome)
### [Docs and Demo](http://github.hubspot.com/odometer)
