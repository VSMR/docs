# ブラウザのサポート状況・音質について

VSMRは最大で左右2チャンネル・Opus Codec・500kbpsで音声のやり取りが可能です。

### VSMRはGoogleChromeを推奨します💪(iPhone / iPadではSafari)

注意！：iPhone / iPadでは、Safari以外のブラウザで使用することができません。また、Safariでは現在モノラル音声しか送受信できません。

また、VSMRの動作・バグ修正等は**GoogleChromeのみ**をサポートしています。GoogleChrome以外のブラウザで生じた不具合に関しては基本的にサポートしません。



## ブラウザ対応表

| 送信側                  | 受信側                 | 音                                                           |
| ----------------------- | ---------------------- | ------------------------------------------------------------ |
| [Win]Chrome             | [Win]Chrome            | ◎ / Stereo Opus 480～500kbps                                 |
| [Win]Chrome             | [Win]Firefox           | ◎ / Stereo Opus 480～500kbps                                 |
| [Win]Firefox            | [Win]Chrome            | ×(通信エラー) / ERROR PeerJS:  Error: (InvalidModificationError) Changing the media-type of m-sections is not allowed |
| [Win]Chrome             | [MacOS Catalina]Safari | △ / Mono Opus 54～60kbps(webrtcのByteSendの値を目視)         |
| [Mac]Chrome             | [Win]Chrome            | △ / Mono Opus 54～60kbps(webrtcのByteSendの値を目視)         |
| [Win]Chrome             | [MacOS Catalina]Chrome | ◎ / Stereo Opus 500kbps                                      |
| [Win]Firefox            | [Mac]Safari            | ×(通信エラー) / ERROR PeerJS:  Error: (InvalidModificationError) Changing the media-type of m-sections is not allowed |
| [Mac]Safari             | [Win]Firefox           | △ / Mono Opus (bit rateは未確認)                             |
| [iPhone]Safari          | [Win]Chrome            | △ / Mono Opus 54～60kbps(webrtcのByteSendの値を目視)<br />残念ながら手持ちの環境で使えるステレオマイクがなかった |
| [iPhone]Chrome          |                        | × / getUserMedia();に非対応                                  |
| [iPhone]Firefox         |                        | × / getUserMedia();に非対応                                  |
| [iPhone]DolphinBrowser  |                        | × / getUserMedia();に非対応                                  |
| [iPhone]Smooz(公開停止) |                        | × / getUserMedia();に非対応                                  |
| [Win]Chrome             | [Android]Chrome        | ◎ / Stereo Opus 500kbps (やや遅いような気がする)             |



## どのブラウザの組み合わせで通信できるかどうか検証した結果

* Firefoxから通話をかけることはできない(受信はできる)
* Safariを介すと音がモノラルになる(SDPの違い)
* GoogleChromeならWin / Mac 問わず高音質で通信できる(もちろんステレオマイク・ ステレオイヤホンは必須です)
* Google Chrome同士では、相手がステレオマイクであればステレオで音が聞こえます

* ネットワーク回線が遅い / pingが遅い・ネットワーク間の通信経路が長ければ長いほど遅延していきます(仕方がないね…)

