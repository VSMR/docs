# VSMR | Virtual ASMR
v2: ![](https://img.shields.io/badge/Version-2.13-green) ![](https://img.shields.io/badge/Build-Stopped-red)  
v3: ![](https://img.shields.io/badge/Version-3.2.4-green) ![](https://img.shields.io/badge/Build-Canceled-red)  
v4: ![](https://img.shields.io/badge/Version-4.8.0-green) ![](https://img.shields.io/badge/Dev-Passing-green)

## Announcements (VSMR will come back again.)
#### VSMR Site
coming soon -> [https://vsmr.app](https://vsmr.app)  
v4 -> [https://v4.vsmr.app/](https://v4.vsmr.app/)

#### A new version of VSMR is currently in development

## About

**VSMR is a voice chat project for binaural collaboration on the Internet**  
**VSMRはインターネットでバイノーラル音声を やりとりすることのできるボイスチャットサービスです**

🎈 **Version 4.8 is released!!** 🎈 [https://v4.vsmr.app/](https://v4.vsmr.app/)

## What is VSMR?

VSMRはインターネットでバイノーラル音声をやり取りできるボイスチャットサービスです。VSMRは、VirtualとASMRの言葉を掛け合わせたもので、主にバーチャルYouTuberのバイノーラルコラボ配信で使用することを目的として開発されました。今までのバイノーラル音声コラボでは、実際に同じ場所でバイノーラルをしたり、netduettoβのような特別なアプリをインストールして行われてきましたが、VSMRではWebブラウザ上で簡単に音声のやり取りができるようになります。

## How to use?

💪VSMRはGoogleChromeを推奨します

🚫iPhone / iPadはSafari以外使用不可・ステレオ通話対応していません

🖋使い方：[HowToUse.md](HowToUse.md)に記載されています

❓よくある質問：[FAQ.md](FAQ.md) に記載されています

## Towards the Official Version
In the official version of VSMR, the following features are planned to be added:

High Priority:
* Room feature (API coding for the room server is done)
* Easier multi-person calls
* UI update (redesigning the current UI and implementing Dark Mode using React Material UI)
* Name display feature (to be implemented using socket.io and roomAPI)
* Stable microphone device management (allowing device changes during calls without issues)
* Source code release (currently set to private)
* Release of source code for developers (currently set to private)
* Change audio bitrate during calls (requires checking WebRTC specifications)
* ~~Function to check if VSMR is being used during streaming (to aggregate how VSMR is being used)~~
* ~~Latency measurement~~ (measured: approximately 80ms latency, 230-260ms faster than Discord https://twitter.com/398noetan/status/1339253964122943488?s=20 )
* Speech to Text feature (automatic conversion of call audio to text ~~by the end of 2021 using Julius~~)
* Donation feature (considering options like Booth due to restrictions on personal remittances in Japan)

Low Priority:
* License: [GPLv3.0 License](LICENSE)

## Bugs and Requests

For bugs, issues, improvements, and requests, please submit them to the [issues](https://github.com/398noe/VSMR/issues) on the VSMR repository.  
Share your thoughts on Twitter using [#VSMR](https://twitter.com/search?q=%23VSMR).

## Developer's Twitter Links

[@398noe](https://twitter.com/398noe) / [@398noetan](https://twitter.com/398noetan)

---

**VSMR Project 2020-2024 / GPL v3 License**