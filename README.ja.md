<div align="center">

<img src="https://raw.githubusercontent.com/ryekee/RuaKey-releases/main/docs/dashboard.png" width="820" alt="RuaKey dashboard" />

# ⌨️ RuaKey

**プライバシー最優先の macOS キーボード統計 App。**
*打鍵は見れど、言葉は覗かず*

[![Download latest](https://img.shields.io/github/v/release/ryekee/RuaKey-releases?label=Download&style=for-the-badge&color=fab387)](https://github.com/ryekee/RuaKey-releases/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/ryekee/RuaKey-releases/total?label=downloads&style=for-the-badge&color=a6e3a1)](https://github.com/ryekee/RuaKey-releases/releases)

macOS 15+ · Apple Silicon と Intel · メニューバーに常駐

[English](README.md) | [简体中文](README.zh-Hans.md) | [繁體中文](README.zh-Hant.md) | 日本語

</div>

---

RuaKey はキーボード（とマウス）の操作を、**この Mac だけに残る**すっきりした統計に変えます。どれだけ速く打っているか、どのキーやショートカットに頼っているか、打鍵がどのアプリに費やされているか、そしてそれらが時間とともにどう変わっていくか。

数えるのは**メタデータだけ**——キーのカテゴリ、キーごとの回数、修飾キーの組み合わせ——すべて**日単位で集約**します。キーの順序やタイミングは一切保存しないため、入力した内容を復元することは物理的に**できません**。

## 🔒 プライバシーがすべて

- **入力データがこの Mac から出ることはありません**。テレメトリーも、分析 SDK も、クラウド同期もなし。
- **打鍵の内容は決して記録しません**——あるのはカテゴリと日別のキーごとの回数だけで、（時刻、キー）の並びは保存しません。
- **物理キーボードごとに集計**——Apple の `IOHIDManager` により、システム全体のイベントストリームから拾うのではなく、デバイス単位でデータをまとめます。
- 通信は GitHub への更新確認*だけ*——それもオフにできます。

> 保存されるデータベースに文字列フィールドはありません。日別のカテゴリ集計から言葉を復元する方法は、そもそも存在しません。

## ✨ できること

- **📊 ダッシュボード**——今日 / 7 日 / 30 日 / 累計の合計、ライブとピークの KPM、削除率、連続日数、時間帯別と曜日別のパターン、そして一年分のアクティビティカレンダー。
- **⌨️ キーボードヒートマップ**——よく打つキーを実物のキーボードの上に描画。配列は **MacBook · 75% · TKL · Alice · HHKB** に対応。
- **🖱️ マウス**——クリックとスクロールの回数に加えて、ディスプレイごとの滑らかなクリックヒートマップ（座標は取得時に量子化され、生の位置がディスクに書かれることはありません）。
- **📱 アプリ別**——打鍵とクリックがどのアプリに費やされているか。
- **📈 7 日間比較**——どの数値にも、今日と直近 7 日間の対比が付きます。
- **🎉 マイルストーン紙吹雪**——7 日間ベストを更新したら全画面でお祝い。
- **🌐 四つの言語**——English、简体中文、繁體中文、日本語。
- **🔄 自動アップデート**——新しいバージョンは自動でインストールされます。

すべてはダークなターミナル / ダッシュボードの美学の中に——琥珀と緑、Departure Mono、密度の高い計器風パネル。

## 📊 データの見方は二つ

<img src="https://raw.githubusercontent.com/ryekee/RuaKey-releases/main/docs/popover.png" align="right" width="300" alt="Menu bar popover" />

**ウィンドウ**はじっくり見る場所——合計、速度、ヒートマップ、アプリ別の内訳、長期トレンドを、一枚のターミナル風ダッシュボードで。

**メニューバー**はひと目で確認する場所——アイコンをクリックすれば、今日の打鍵とクリック、ピーク KPM、削除率、トップのキー / コンボ / キーボード / アプリ、さらに HUD・KPM モード・一時停止のスイッチまで。ウィンドウを開く必要はありません。

<br clear="all"/>

## 🎚️ ライブ HUD

作業中の画面にそっと浮かぶ小さなストリップ——**ライブ KPM**、**いま押したキー**、**今日の合計**が、打つそばから更新されます：

<div align="center">
<img src="https://raw.githubusercontent.com/ryekee/RuaKey-releases/main/docs/hud.gif" width="600" alt="RuaKey live HUD" />
</div>

- 打ち始めた瞬間に**自動で現れ**、手が止まると**フェードアウト**。
- **ポインタをよけます**——近づくとすっと脇へ退き、下の内容を隠しません（設定でオフにできます）。
- 画面上の六つの位置に固定でき、非表示までのアイドル時間も調整できます。
- **自分好みに**——モジュールは表示・非表示・ドラッグでの並べ替えに対応。KPM が上がるほど速く打つ**タイピングネコ**もいます。

## 📥 インストール

1. **[最新の `.dmg`](https://github.com/ryekee/RuaKey-releases/releases/latest)** をダウンロードして、**RuaKey** を「アプリケーション」へドラッグ。
2. 初回起動は**右クリック → 開く**で Gatekeeper を通します（App は ad-hoc 署名で、公証はされていません）。
3. 求められたら**入力モニタリング**を許可し、**終了して再起動**——macOS の仕様により、再起動しないと有効になりません。

0.3 以降、アップデートは自動でインストールされます。ひとつだけ注意：App は ad-hoc 署名（公証なし）のため、更新後に macOS が**入力モニタリング**の許可を忘れることがあります——**設定 ▸ プライバシー**に、ワンステップで戻せるガイドがあります。

---

<div align="center">
<sub>RuaKey が記録するのは回数だけで、内容ではありません。あなたの言葉はあなたのものです。</sub>
</div>
