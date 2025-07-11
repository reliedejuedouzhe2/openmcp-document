# 変更履歴

## [main] 0.1.1
- UbuntuへのSSH接続時のバグを修正
- Pythonプロジェクトでopenmcpをクリックして接続する際の初期化パラメータエラーを修正
- service層のmcp接続再利用技術を廃止し、リフレッシュ不能問題を防止
- 接続後、ウェルカム画面でデバッグオプションが選択できないバグを修正

## [main] 0.1.0
- 新機能: 複数mcpサーバーへの同時接続をサポート
- 新機能: プロトコル内容を更新し、streamable httpプロトコルをサポート（今後SSE接続方式を段階的に置換）
- issue#16実装: uv作成のpyプロジェクト向け特別サポート（自動初期化、mcpを.venv/bin/mcpに自動設定）
- npm作成のjs/tsプロジェクト向け特別サポート: 自動プロジェクト初期化
- websearch設定を削除、parallel_tool_calls設定を追加（デフォルトtrue: 単一応答内での複数ツール呼び出し許可）
- openmcp接続モジュールインフラをリファクタリング、詳細なログシステムを実装
- issue#15実装: コピー不能問題
- issue#14実装: ログ消去ボタン追加

## [main] 0.0.9
- 0.0.8で導入されたバグ修正: system promptがインデックスではなく実際の内容を返すように
- 新しいリリースパイプラインをテスト

## [main] 0.0.8
- 大規模モデルAPIテスト時のエラーレポートを強化
- 0.0.7で導入されたバグ修正: 会話編集が送信できない問題
- リッチテキストエディタの貼り付けスタイル問題を修正
- リッチテキストエディタの空文字送信問題を修正
- ストリーミング中のfunction calling時、マルチツールインデックスによるJSON Schemaデシリアライズ失敗を修正
- 大規模モデルの重複エラーメッセージ問題を修正
- 新機能: 単一会話での複数ツール同時呼び出しをサポート
- UI: コードハイライトのスクロールバーを最適化
- 新機能: resources/listプロトコルコンテンツのクリック直接レンダリングを実装
- 新機能: resources/prompts/toolsのJSON結果表示にハイライトをサポート

## [main] 0.0.7
- ページレイアウトを最適化し、デバッグウィンドウの表示領域を拡大
- デフォルトコンテキスト長を10→20に拡張
- 「一般オプション」に「MCPツール最大呼び出し時間(秒)」を追加
- リッチテキスト入力欄をサポート、大規模prompt engineeringデバッグ作業が可能に

## [main] 0.0.6
- サーバー名特殊文字による保存不具合を修正
- プラグインモードで左パネルの「MCP接続(ワークスペース)」ビューのCRUD操作を実現
- 「インストール済みMCPサーバー」を追加（グローバル範囲mcp server管理）
- ガイドページを追加
- オフラインOCR不能問題を修正
- グローバルインストールmcpサーバーのname更新問題を修正

## [main] 0.0.5
- 開いたことのあるファイルプロジェクトの管理をサポート
- ユーザー別サーバーデバッグ作業内容の保存をサポート
- 連続ツール呼び出しとエラー警告表示を実装
- 小型ローカルオブジェクトデータベースを実装（会話生成マルチメディアの永続化）
- 呼び出し結果のワンクリック再現をサポート
- 中間結果の編集をサポート
- system promptの保存・編集をサポート

## [main] 0.0.4
- モデル選択後確認クリックでdeepseekに戻るバグを修正
- mcpプロジェクト初期化時ツールが空になるバグを修正
- 再接続不能問題を修正
- サードパーティOpenAI互換モデルサービスのカスタマイズをサポート

## [main] 0.0.3
- メッセージごとのコスト統計情報を追加
- 初期化ページルートがdebugでない場合の白画面バグを修正

## [main] 0.0.2
- ページレイアウトを最適化
- タブ更新後の表示不能バグを解決
- 入力コンポーネントでEnter押下時の黒画面バグを解決
- より完全で便利な開発スクリプトを実装

## [main] 0.0.1
- openmcp基本inspector機能を完成
- 設定読み込み/保存、大規模モデル設定を実装
- タブ自動保存機能を実装
- 大規模モデル会話ウィンドウとツール呼び出しを実装
- vscodeとtraeのサポートを実装