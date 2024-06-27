# Frequently Asked Questions

## "Sorry, you cannot use VSMR" message appears...

Your browser may not support VSMR for various reasons (e.g., inability to access the microphone). VSMR is recommended to be used with Google Chrome. (For iPhone/iPad, VSMR is only available on Safari). While iPhone does not currently support binaural audio transmission, you can still connect using audio through Safari. Please refer to `BrowserSupport.md` to check browser compatibility.

## My voice is not echoed back when accessing the site

When accessing VSMR, your voice should be echoed back each time the default device is selected. After setting the microphone, press the change microphone button. If the microphone is not powered on, the device driver has issues, or if a mixer is muted, you might not hear any sound.

## Unable to connect even after entering the other person's ID

* Did you enter the correct ID? Typing errors with characters like `1` (one), `l` (lowercase L), and `I` (uppercase I) are common. Please double-check.
* Refreshing the browser page changes the ID each time. This ID cannot be fixed. If one party refreshes the browser before the other connects, the connection will not be established (the ID changes upon refresh, so closing the browser tab immediately disconnects). Ensure the page is not refreshed.
* When copying the ID, accidentally adding spaces at the beginning or end can result in an incorrect ID, preventing connection.
* Occasionally, the generated ID may not be usable. (This can happen during automatic ID generation.)
  * <small>For example, IDs starting with - (hyphen) or _ (underscore) or containing consecutive such symbols can cause issues. In such cases, refresh the browser to generate a new ID.</small>
* There could also be server-side errors. We apologize for any inconvenience caused.

## My (or the other person's) voice doesn't sound binaural!

* **VSMR does not automatically convert audio from any microphone to binaural audio.** To send binaural audio, **no part of the transmission path should be mono before it reaches the VSMR page.**
  * For instance, using a mono microphone, an audio interface not supporting stereo input, connecting to a PC's mono microphone input, or using a virtual audio cable driver that only supports mono (though unlikely).
  * Even with a binaural microphone, if using a cheap audio interface that only supports mono output, the PC will only capture mono sound.
  * Despite being mono, VSMR's audio transmission bit rate is up to 500kbps, providing much better sound quality than services like Discord.
  * If you use two mono microphones and a mixer that outputs stereo sound, you should be able to send binaural audio through VSMR (not yet verified).
* Recommended options include using a stereo-capable microphone. Affordable options are ROLAND CS-10EM, TASCAM DR series, ZOOM H series, and dummy head microphones like 3dio freespace or SR3D. (The developer, Sakubanoya, uses H3-VR)

VSMR is designed for use by creators of audio doujin works, binaural/ASMR streams, etc., so most users should already meet these requirements.