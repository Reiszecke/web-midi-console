Fork from https://github.com/benschmaus/web-midi-console because I needed a convenient way of sending hexadecimal values without having to manually convert them to decimals. Replace `hexTarget = "TD-3" ` in index.js with whatever your target is gonna be and you can simply enter something like `AA 0B 1C` in the hexBox and it will turn the input into `device("TD-3").raw([170,11,28])`. So basically you don't have to convert and type everything out. It's a small utility that I needed to reverse-engineer above-mentioned synth.

Unless you need that, you are probably better off using the original repo.

Original Readme below:

# web-midi-console
Web MIDI Chrome app for viewing messages from connected MIDI devices and sending messages to them.

You can try out the Web MIDI Console at [factotumo.com/web-midi-console/](https://factotumo.com/web-midi-console/).

If you'd like to develop locally, do the following.

1. ```$ git clone git@github.com:benschmaus/web-midi-console.git```
2. ``` $ cd web-midi-console && python -m SimpleHTTPServer 8000```

You can then open http://localhost:8000 in your browser to see a locally running console.  The document root of the server is the directory the server is started from.  In the above example, it would be ```<your-checkout-dir>/web-midi-console```.

Feedback, feature requests, etc. are welcome.
