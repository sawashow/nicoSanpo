# AI_CONTEXT.md

## プロジェクト概要
nicoSanpo (DriveSpotter) - ドライブ中の記憶や位置情報から曖昧な店舗・スポットをAIで特定・記録するWebアプリケーション。

## 技術構成
- 単一HTML構成 (`index.html`)
- Vanilla JS, Tailwind CSS (CDN), Lucide Icons
- Gemini API (`gemini-2.5-flash` / `gemini-flash-latest`)

## 直近の変更内容
- 送信されたコンソールエラーログの通り、`index.html` のファイル末尾付近で `<script>` 閉じタグが一部抜け落ちていたため JavaScript 全体で構文エラーが発生し、`captureSpot is not defined` エラーを引き起こしていた根本原因を修正。
- PWA Manifest の Data URI を完全エンコード表記に統一し、ブラウザコンソールの Manifest Syntax Error 警告を解消。
