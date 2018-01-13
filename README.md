Here is an implementation of HttpUrlConnection developed in Android Studio that use the code taken from
http://www.codexpedia.com/android/asynctask-and-httpurlconnection-sample-in-android/

Takes the weather information with an api and it posts the field text to a nodeJs server:

/server.js/

var express = require('express');
var app = express();

app.get('/*', function (req, res) {
    console.log(req.url);
    console.log(req.params);
    res.send('OK!');
})

var server = app.listen(8081, function () {

    var host = server.address().address
    var port = server.address().port

    console.log("Example app listening at http://%s:%s", host, port)
})
