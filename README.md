node-google-text-to-speech
==========================

Google Text-To-Speech for node.js

A small library for translating text-to-speech service for google.

## Installation

  npm install node-google-text-to-speech --save

## Usage

  var tts = require('node-google-text-to-speech')
  
  tts.translate('en', 'dog', function(result) {
  	console.log(result); 
  	if(result.success) { //check for success
  		socket.emit('ttsResult', 'audio' : result.data); //emit the audio to client
  	}
  });

## Release History

* 0.1.0 Initial release