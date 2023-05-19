# dataML

var DecompressZip = require('decompress-zip');
var unzipper = new DecompressZip(filename)

unzipper.on('error', function (err) {
    console.log('Caught an error');
});

unzipper.on('list', function (files) {
    console.log('The archive contains:');
    console.log(files);
});

unzipper.list();
