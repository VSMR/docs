# Browser Support and Audio Quality

VSMR supports audio transmission with up to two channels, using the Opus Codec at 500kbps.

### VSMR recommends using Google Chrome💪 (Safari for iPhone/iPad)

Note! On iPhone/iPad, VSMR cannot be used with browsers other than Safari. Additionally, Safari currently only supports mono audio transmission.

Moreover, VSMR's functionality and bug fixes are only supported on **Google Chrome**. We generally do not support issues that occur on browsers other than Google Chrome.

## Browser Compatibility Table

| Sender                 | Receiver               | Audio                                                        |
| ---------------------- | ---------------------- | ------------------------------------------------------------ |
| [Win]Chrome            | [Win]Chrome            | ◎ / Stereo Opus 480-500kbps                                  |
| [Win]Chrome            | [Win]Firefox           | ◎ / Stereo Opus 480-500kbps                                  |
| [Win]Firefox           | [Win]Chrome            | × (Communication Error) / ERROR PeerJS: Error: (InvalidModificationError) Changing the media-type of m-sections is not allowed |
| [Win]Chrome            | [MacOS Catalina]Safari | △ / Mono Opus 54-60kbps (based on observed webrtc ByteSend values) |
| [Mac]Chrome            | [Win]Chrome            | △ / Mono Opus 54-60kbps (based on observed webrtc ByteSend values) |
| [Win]Chrome            | [MacOS Catalina]Chrome | ◎ / Stereo Opus 500kbps                                      |
| [Win]Firefox           | [Mac]Safari            | × (Communication Error) / ERROR PeerJS: Error: (InvalidModificationError) Changing the media-type of m-sections is not allowed |
| [Mac]Safari            | [Win]Firefox           | △ / Mono Opus (bit rate unconfirmed)                         |
| [iPhone]Safari         | [Win]Chrome            | △ / Mono Opus 54-60kbps (based on observed webrtc ByteSend values) <br />Unfortunately, no stereo microphone was available in the current environment |
| [iPhone]Chrome         |                        | × / Not supported by getUserMedia();                         |
| [iPhone]Firefox        |                        | × / Not supported by getUserMedia();                         |
| [iPhone]DolphinBrowser |                        | × / Not supported by getUserMedia();                         |
| [iPhone]Smooz (discontinued) |                  | × / Not supported by getUserMedia();                         |
| [Win]Chrome            | [Android]Chrome        | ◎ / Stereo Opus 500kbps (appears slightly slow)              |

## Summary of Browser Compatibility Tests

* Calls cannot be made from Firefox (but can be received)
* Audio becomes mono when using Safari (due to SDP differences)
* High-quality communication is possible with Google Chrome on both Win/Mac (Stereo microphones and earphones are required)
* When using Google Chrome, if the other party has a stereo microphone, the audio will be in stereo

* Network delays increase with slower networks, higher ping, or longer network communication paths (inevitable...)