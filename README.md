# Justin

Full-stack developer based in Japan. Looking for a junior dev role.

I build web apps and tools — mostly TypeScript/Next.js on the frontend, Python and occasionally Rust on the backend. A lot of my work has been Japanese-market facing.

---

## Main Projects

### Dream Docs — Document Delivery Platform
> End-to-end encrypted document submission system built for Japanese high school students applying to a Canadian study abroad program.

Built in two iterations:

**v1** — Split architecture: a Next.js student-facing web app paired with a native Rust/Iced desktop app for administrators. Files are encrypted client-side (AES-256-GCM + RSA-OAEP) before they ever leave the browser. The admin desktop app holds the RSA private key and decrypts documents locally — plaintext never touches the server.

**v2** — Consolidated both student and admin flows into a single Next.js app after recognising the split architecture was overkill. Added a custom form builder, richer admin dashboard, and role-based access control.

| Repo | Description |
|---|---|
| [dream-docs-client](https://github.com/JAC-1/dream-docs-client) | v1 — Student web app (Next.js, TypeScript, E2E encryption) |
| [dream-docs-admin-iced](https://github.com/JAC-1/dream-docs-admin-iced) | v1 — Admin desktop app (Rust, Iced) |
| [dd-mk2](https://github.com/JAC-1/dd-mk2) | v2 — Unified full-stack app (Next.js 15, Supabase, Drizzle ORM) |

> 📸 Screenshots coming soon

---

### ISBN Scraper
> Takes a spreadsheet of ISBNs, scrapes book metadata from Japanese and international book sites, and outputs a populated Excel file.

Built with Node.js and Puppeteer. Reads from `RawBarcodes.xlsx`, skips already-cached entries, scrapes Booklog and Bookfinder for title/author/publisher/description, and writes results to a local JSON database and output spreadsheet.

**Stack:** Node.js · Puppeteer · ExcelJS

[→ isbnscraper](https://github.com/JAC-1/isbnscraper)

---

### NFD — NIT Factbook Downloader
> Automated pipeline that finds and downloads FactBook PDFs from Japanese university websites.

Uses the DuckDuckGo API to find candidate links, feeds them to Claude Haiku to evaluate relevance, then uses Playwright to navigate and download. Includes cost logging per university processed (~$0.31 per 1000 universities at step 4).

**Stack:** Python · Playwright · Claude API · DuckDuckGo API · Poetry

[→ nfd](https://github.com/JAC-1/nfd)

---

## Other Projects

| Repo | Description | Stack |
|---|---|---|
| [awkward-pywright](https://github.com/JAC-1/awkward-pywright/tree/hunt-and-search) | Earlier iteration of the factbook finder — Playwright hunting for search bars across university sites | Python · Playwright |
| [elsc-library-inventory-checker](https://github.com/JAC-1/elsc-library-inventory-checker) | Desktop tool for scanning and editing a library book inventory from Excel files | Python · EEL · Pandas |
| [rude-mistral](https://github.com/JAC-1/rude-mistral) | Calling a custom Mistral agent (rude British persona) via TypeScript/Bun | TypeScript · Bun · Mistral AI |

---

## Stack

`TypeScript` `Next.js` `React` `Python` `Rust` `Node.js` `PostgreSQL` `Supabase` `Tailwind CSS` `Playwright` `Docker`

---
---

# 日本語 / Japanese

# Justin

日本在住のフルスタックエンジニアです。ジュニア開発職を希望しています。

Web アプリやツールの開発を行っており、フロントエンドは主に TypeScript/Next.js、バックエンドは Python や Rust を使用しています。日本市場向けのプロジェクトを多く手がけています。

---

## メインプロジェクト

### Dream Docs — ドキュメント配信プラットフォーム
> カナダ留学プログラムに申請する日本人高校生向けの、エンドツーエンド暗号化ドキュメント提出システムです。

2つのバージョンで開発しました：

**v1** — 分割アーキテクチャ：学生向け Next.js Web アプリと、管理者向け Rust/Iced 製ネイティブデスクトップアプリの組み合わせ。ファイルはブラウザを離れる前にクライアント側で暗号化（AES-256-GCM + RSA-OAEP）されます。管理者アプリが RSA 秘密鍵を保持しローカルで復号するため、平文がサーバーに触れることはありません。

**v2** — 分割アーキテクチャが過剰だと判断し、学生・管理者の両フローを単一の Next.js アプリに統合。カスタムフォームビルダー、充実した管理ダッシュボード、ロールベースアクセス制御を追加しました。

| リポジトリ | 説明 |
|---|---|
| [dream-docs-client](https://github.com/JAC-1/dream-docs-client) | v1 — 学生向け Web アプリ（Next.js、TypeScript、E2E 暗号化） |
| [dream-docs-admin-iced](https://github.com/JAC-1/dream-docs-admin-iced) | v1 — 管理者向けデスクトップアプリ（Rust、Iced） |
| [dd-mk2](https://github.com/JAC-1/dd-mk2) | v2 — 統合フルスタックアプリ（Next.js 15、Supabase、Drizzle ORM） |

> スクリーンショットは近日公開予定

---

### ISBN スクレイパー
> ISBN のスプレッドシートを読み込み、日本語・海外の書籍サイトから書誌情報を取得して Excel ファイルに出力するツールです。

Node.js と Puppeteer で構築。`RawBarcodes.xlsx` から読み込み、キャッシュ済みエントリはスキップ、Booklog と Bookfinder からタイトル・著者・出版社・説明を取得し、ローカルの JSON データベースと出力スプレッドシートに書き込みます。

**技術スタック：** Node.js · Puppeteer · ExcelJS

[→ isbnscraper](https://github.com/JAC-1/isbnscraper)

---

### NFD — NIT ファクトブックダウンローダー
> 日本の大学 Web サイトからファクトブック PDF を自動で見つけてダウンロードするパイプラインです。

DuckDuckGo API で候補リンクを検索し、Claude Haiku で関連性を評価、Playwright でナビゲーションとダウンロードを実行します。大学 1 件あたりのコストログを含む（ステップ 4 時点で 1000 大学あたり約 $0.31）。

**技術スタック：** Python · Playwright · Claude API · DuckDuckGo API · Poetry

[→ nfd](https://github.com/JAC-1/nfd)

---

## その他のプロジェクト

| リポジトリ | 説明 | 技術スタック |
|---|---|---|
| [awkward-pywright](https://github.com/JAC-1/awkward-pywright/tree/hunt-and-search) | ファクトブック検索の旧バージョン — Playwright で大学サイトの検索バーを探索 | Python · Playwright |
| [elsc-library-inventory-checker](https://github.com/JAC-1/elsc-library-inventory-checker) | Excel ファイルから図書館書籍在庫をスキャン・編集するデスクトップツール | Python · EEL · Pandas |
| [rude-mistral](https://github.com/JAC-1/rude-mistral) | TypeScript/Bun でカスタム Mistral エージェント（無礼なイギリス人ペルソナ）を呼び出す | TypeScript · Bun · Mistral AI |

---

## 技術スタック

`TypeScript` `Next.js` `React` `Python` `Rust` `Node.js` `PostgreSQL` `Supabase` `Tailwind CSS` `Playwright` `Docker`
