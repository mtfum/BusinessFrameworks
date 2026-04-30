# Business Frameworks for Claude Code

ビジネスフレームワークを対話的に活用するための Claude Code プラグイン。  
課題に応じた最適なフレームワークを提案し、対話形式でワークシートを完成させます。

## 収録フレームワーク（9カテゴリ・73種）

| カテゴリ | スキル名 | 収録数 | 主なフレームワーク |
|---------|---------|:-----:|----------------|
| 問題発見・課題定義 | `problem` | 9 | As is／To be, なぜなぜ分析, ロジックツリー, MECE, イシューツリー |
| マクロ環境・業界分析 | `market` | 7 | PEST分析, ファイブフォース, 3C分析, SWOT, バリューチェーン |
| 顧客理解・市場セグメント | `customer` | 8 | ペルソナ, 共感マップ, カスタマージャーニー, ジョブ理論, STP |
| アイデア発想・評価 | `idea` | 9 | マンダラート, SCAMPER, デザイン思考, オズボーンのチェックリスト |
| 戦略立案・ビジネスモデル設計 | `strategy` | 10 | BMC, リーンキャンバス, ブルーオーシャン, 4P分析, AIDMA |
| 目標設定・実行管理 | `execution` | 9 | OKR, KPIツリー, SMART, AARRR, バランスト・スコアカード |
| 業務改善・プロセス最適化 | `improvement` | 8 | PDCA, KPT, YWT, RACI, ECRS |
| 組織・チームマネジメント | `organization` | 9 | MVV, Will／Can／Must, ジョハリの窓, GROWモデル |
| 伝達・プレゼンテーション | `communication` | 4 | PREP, TAPS, ピラミッドストラクチャー, エレベーターピッチ |

## インストール

```bash
claude /plugin install github:mtfum/BusinessFrameworks
```

## 使い方

### メインメニューから選ぶ

```
/business-frameworks:framework
```

課題を伝えると、最適なフレームワークを提案してくれます。

### カテゴリを直接指定

```
/business-frameworks:strategy
/business-frameworks:problem
/business-frameworks:customer
```

### フレームワーク名を指定

```
/business-frameworks:strategy SWOT分析
/business-frameworks:idea マンダラート
/business-frameworks:execution OKR
```

### ローカルでテスト

```bash
git clone https://github.com/mtfum/BusinessFrameworks.git
cd BusinessFrameworks
claude --plugin-dir .
```

## ディレクトリ構成

```
.claude-plugin/
  plugin.json           # プラグインマニフェスト
skills/
  framework/SKILL.md    # メインエントリ（一覧・自動提案）
  problem/SKILL.md      # 問題発見・課題定義
  market/SKILL.md       # マクロ環境・業界分析
  customer/SKILL.md     # 顧客理解・市場セグメント
  idea/SKILL.md         # アイデア発想・評価
  strategy/SKILL.md     # 戦略立案・ビジネスモデル設計
  execution/SKILL.md    # 目標設定・実行管理
  improvement/SKILL.md  # 業務改善・プロセス最適化
  organization/SKILL.md # 組織・チームマネジメント
  communication/SKILL.md # 伝達・プレゼンテーション
```

## ライセンス

MIT
