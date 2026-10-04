# Minutes Ago

**Record the meeting after it happened.** Minutes Ago is a menu bar app for Mac that keeps recording your microphone on this Mac, so you can save the part you need afterwards — audio, transcript, speakers and meeting minutes. By default, neither audio nor transcripts leave your Mac.

🌐 [Website](https://www.kurokoto.com/minutesago/) · 📥 [Download the latest release](https://github.com/KurokotoLab/MinutesAgo/releases/latest/download/MinutesAgo.dmg) · 📖 [Guide](https://www.kurokoto.com/minutesago/guide/) · 🇯🇵 [日本語](#日本語)

This repository hosts the releases of the **direct-download version** (and its update feed). It contains no source code.

## What it does

- **Always recording, only on this Mac.** Keeps the last stretch of microphone audio — 30 minutes to 24 hours, as you set — and deletes older audio and transcripts automatically.
- **Transcribes on this Mac** with Apple's speech recognition.
- **Save it afterwards.** Save the last few minutes, or any range from the timeline, as audio and a transcript.
- **Speakers and minutes.** Identifies speakers, and writes meeting minutes with Apple Intelligence on this Mac. Other minutes engines ask before anything is sent.
- **App audio (optional).** Records the sound of one app you choose, such as the other side of an online meeting, as a separate track.
- **For agents and scripts.** A local MCP server (off until you turn it on), Shortcuts actions, and the `minutesago` command-line tool, included in this version.

## Requirements

- macOS 27 or later on a Mac with Apple silicon.
- Meeting minutes need Apple Intelligence. Recording, transcription, export and speaker identification work without it.

## Install

1. Download `MinutesAgo.dmg` from the [latest release](https://github.com/KurokotoLab/MinutesAgo/releases/latest).
2. Open the DMG and drag **Minutes Ago** into **Applications**.
3. Open Minutes Ago. A five-page guide walks you through the microphone permission. Recording starts only when you click **Start Recording**.

The app and the disk image are signed with a Developer ID and notarized by Apple. macOS asks for system audio recording only when you choose an app under app audio. Details: [Getting Started](https://www.kurokoto.com/minutesago/guide/getting-started/).

## Updates

Choose **Check for Updates…** in the menu. Updates are delivered from this repository's releases with [Sparkle](https://sparkle-project.org/) and are signed. Automatic checks are off unless you allow them, and an update is installed only when you choose to install it.

## Free and paid

- The download is free. Saving, copying and minutes on this Mac for the last 30 minutes are free, with no limit on how many times.
- Older audio, speaker names, the app audio track, other minutes engines, and taking things out through agents or the command-line tool (beyond the buffer status and the last 30 minutes of transcript) can be tried 5 times. A license removes the limit.
- A license is a one-time purchase with no subscription, sold in US dollars through [Polar](https://polar.sh/). It can be active on up to 3 Macs at a time, and refunds are available within 14 days of purchase. Current prices: [Pricing](https://www.kurokoto.com/minutesago/#pricing).
- Minutes Ago is also planned for the Mac App Store. Purchases don't carry over between the App Store version and this version.

## Command-line tool

The tool is at `/Applications/Minutes Ago.app/Contents/MacOS/minutesago`. **Agent access › Command line tool…** in the menu shows how to put it on your PATH. Usage, subcommands and exit codes: [Command-line tool (direct version)](https://www.kurokoto.com/minutesago/guide/agents-and-shortcuts/#command-line-tool-direct-version).

## Privacy

Audio and transcripts stay on this Mac unless you choose an outside minutes engine. This version also contacts Polar (api.polar.sh) to activate and check a license, and GitHub to check for updates. Every connection is listed in [Connections off your Mac](https://www.kurokoto.com/minutesago/guide/data-and-privacy/#connections-off-your-mac-this-is-all-of-them).

## Uninstall

1. If you activated a license, choose **License… › Deactivate This Mac** to free the slot.
2. Choose **Erase everything** in the menu.
3. Quit Minutes Ago and move it to the Trash.
4. To remove the rest, delete `~/Library/Containers/com.kurokoto.minutesago.direct/` and `~/Library/Group Containers/UY6Q9BGBWY.com.kurokoto.minutesago/`. If you added the command-line tool to `/usr/local/bin`, run `sudo rm /usr/local/bin/minutesago`.

Exported files stay in the folder you chose.

## Support

- Guide and FAQ: <https://www.kurokoto.com/minutesago/guide/>
- Questions: [support@kurokoto.com](mailto:support@kurokoto.com)
- [Terms of Use](https://www.kurokoto.com/legal/minutesago/terms/) · [Privacy Policy](https://www.kurokoto.com/legal/minutesago/privacy/)

---

## 日本語

**会議が終わってから、録音する。** Minutes Ago は、Mac のマイクをこの Mac の中で録り続け、必要になった部分をあとから保存できるメニューバーのアプリです。音声・文字起こし・話者・議事録を残せます。音声も文字起こしも、既定ではこの Mac を出ません。

🌐 [Web サイト](https://www.kurokoto.com/ja/minutesago/) · 📥 [最新版をダウンロード](https://github.com/KurokotoLab/MinutesAgo/releases/latest/download/MinutesAgo.dmg) · 📖 [ガイド](https://www.kurokoto.com/ja/minutesago/guide/)

このリポジトリは**直販版**のリリース（とアップデートの配信元）です。ソースコードは置いていません。

### できること

- **この Mac の中で録り続ける。** マイクの音声を設定した長さ（30 分〜24 時間）だけ保持し、古い音声と文字起こしは自動で消します。
- **この Mac で文字起こし**（Apple の音声認識）。
- **あとから保存。** 直近の数分やタイムラインで選んだ範囲を、音声と文字起こしで書き出せます。
- **話者と議事録。** 話者を分け、この Mac の Apple Intelligence で議事録を作ります。ほかの議事録エンジンは、送る前に確認します。
- **アプリ音声（任意）。** 選んだ 1 つのアプリの音（オンライン会議の相手の声など）を別のトラックで録れます。
- **エージェントとスクリプト。** ローカルの MCP サーバー（オンにするまでオフ）、ショートカットのアクション、この版に同梱のコマンドラインツール `minutesago`。

### 動作環境

- macOS 27 以降、Apple silicon の Mac。
- 議事録には Apple Intelligence が必要です。録音・文字起こし・書き出し・話者の識別はなくても使えます。

### インストール

1. [最新リリース](https://github.com/KurokotoLab/MinutesAgo/releases/latest)から `MinutesAgo.dmg` をダウンロードします。
2. DMG を開き、**Minutes Ago** を **アプリケーション** にドラッグします。
3. Minutes Ago を開くと、5 ページの案内でマイクの許可を進めます。録音は **録音を開始** を押したときだけ始まります。

アプリとディスクイメージは Developer ID で署名し、Apple の公証を受けています。システムオーディオ録音の許可は、アプリ音声でアプリを選んだときだけ求めます。詳しくは[はじめに](https://www.kurokoto.com/ja/minutesago/guide/getting-started/)。

### アップデート

メニューの **アップデートを確認…** から。このリポジトリのリリースから [Sparkle](https://sparkle-project.org/) で配信し、署名を確かめてから入れます。自動の確認は許可したときだけ行い、インストールは利用者が選んだときだけ行います。

### 無料の範囲とライセンス

- ダウンロードは無料です。直近 30 分の書き出し・コピー・この Mac での議事録は、回数の制限なくずっと無料です。
- 30 分より前、話者名、アプリ音声のトラック、ほかの議事録エンジン、エージェントやコマンドラインツールでの取り出し（バッファの状態と直近 30 分の文字起こしは無料）は 5 回まで試せます。ライセンスで制限がなくなります。
- ライセンスは買い切り（サブスクリプションなし）で、[Polar](https://polar.sh/) を通じて米ドル建てで販売します。同時に 3 台の Mac まで有効にでき、購入から 14 日以内は返金できます。価格は[価格の節](https://www.kurokoto.com/ja/minutesago/#pricing)をご覧ください。
- Mac App Store 版も予定しています。App Store 版と直販版の購入は、相互に使えません。

### コマンドラインツール

`/Applications/Minutes Ago.app/Contents/MacOS/minutesago` にあります。PATH への追加はメニューの **エージェント連携 › コマンドラインツール…** に案内があります。使い方・サブコマンド・終了コードは[コマンドラインツール（直販版）](https://www.kurokoto.com/ja/minutesago/guide/agents-and-shortcuts/#コマンドラインツール直販版)。

### プライバシー

外部の議事録エンジンを選ばない限り、音声と文字起こしはこの Mac を出ません。この版はほかに、ライセンスの有効化と確認のために Polar（api.polar.sh）へ、アップデートの確認のために GitHub へ接続します。すべての通信は[Mac の外への通信](https://www.kurokoto.com/ja/minutesago/guide/data-and-privacy/#mac-の外への通信これで全部です)にあります。

### アンインストール

1. ライセンスを有効にしていたら、**ライセンス… › この Mac の登録を解除** で枠を空けます。
2. メニューの **すべて消去** を選びます。
3. Minutes Ago を終了し、ゴミ箱に入れます。
4. 残りも消すなら `~/Library/Containers/com.kurokoto.minutesago.direct/` と `~/Library/Group Containers/UY6Q9BGBWY.com.kurokoto.minutesago/` を削除します。コマンドラインツールを `/usr/local/bin` に入れた場合は `sudo rm /usr/local/bin/minutesago`。

書き出したファイルは、選んだフォルダに残ります。

### サポート

- ガイドと FAQ: <https://www.kurokoto.com/ja/minutesago/guide/>
- お問い合わせ: [support@kurokoto.com](mailto:support@kurokoto.com)
- [利用規約](https://www.kurokoto.com/ja/legal/minutesago/terms/) · [プライバシーポリシー](https://www.kurokoto.com/ja/legal/minutesago/privacy/)

---

<sub>This repository hosts releases only. © 2026 Yuji Kuroko (Kurokoto Lab)</sub>
