# Simple Stats

[![Latest Release](https://badgen.net/github/release/chililikobo/SimpleStats)](https://github.com/chililikobo/SimpleStats/releases/latest)
[![Downloads](https://badgen.net/github/assets-dl/chililikobo/SimpleStats)](https://github.com/chililikobo/SimpleStats/releases/latest)
[![License](https://badgen.net/badge/license/Freeware/purple)](#%E5%88%A9%E7%94%A8%E8%A6%8F%E7%B4%84--terms-of-use)
[![Platform](https://badgen.net/badge/platform/Windows/black)](#%E5%8B%95%E4%BD%9C%E7%92%B0%E5%A2%83--system-requirements)

**Simple Stats** は、PCのリソース状況とネットワーク情報を控えめかつスタイリッシュに表示する、超軽量・単体動作のデスクトップ常駐システムモニターです。  
**Simple Stats** is an ultra-lightweight, standalone desktop telemetry HUD for Windows that visualizes real-time system resources and network diagnostics with minimal overhead.

---

## 主な機能 / Key Features

*   **超低負荷 NativeAOT エンジン / Ultra-Low Footprint**: Win32 API / GDI+ 直描画と .NET 10 NativeAOT により、サードパーティ製UIフレームワーク不使用・実測ワーキングセット約 0.3 MB（プライベート約 7 MB）・ほぼ 0% の CPU 負荷で軽快に動作。
    *   Powered by native Win32 / GDI+ rendering and .NET 10 NativeAOT with zero third-party UI libraries (~0.3 MB working set / ~7 MB private bytes, near-zero CPU).
*   **2つの非干渉モード & 全画面一時停止 / Non-Intrusive Display Modes**: `Win+D` でも消えずタスクバーや `Alt+Tab` に出ない「**壁紙レイヤー固定**」と、マウス接近で自動透過フェードし `Ctrl + Alt` 押下中のみ操作できる「**最前面ゴーストHUD**」を搭載。全画面ゲーム・プレゼン実行中は自動で描画・監視を停止。
    *   Choose between **Wallpaper Layer Mode** (pinned behind windows, survives `Win+D`) and **Ghost Overlay Mode** (click-through with mouse-proximity auto-fade & `Ctrl + Alt` unlock), plus automatic pause on fullscreen apps/games.
*   **高精度テレメトリ & 60秒スパークライン / Accurate Telemetry & 60s Sparklines**: タスクマネージャー準拠の CPU 使用率（`PDH % Processor Utility`）、メモリ、物理ディスク重複排除 I/O、各固定ドライブの使用量・空き容量バー、送受信通信速度（Kbps / Mbps / Gbps）をアークゲージと60秒波形グラフで可視化。
    *   Visualizes Task Manager-aligned CPU utility, RAM, deduplicated physical disk I/O, per-drive Used/Free capacity bars, and network bitrates with arc gauges and 60-second dynamic sparklines.
*   **4テーマ・3レイアウト・3段階フォント / Customizability**: *Obsidian Glass* / *Pure Wallpaper* / *Cyber Cyan* / *Frost Light* の4テーマ、*Standard* / *Minimal Zen* / *Compact Mini* の3種のスリムレイアウト、小・中・大のフォントサイズ切替に対応。
    *   Includes 4 themes, 3 slim layouts, and 3 font sizes (Small / Medium / Large).
*   **NIC自動追従・1クリックコピー・レジストリ不使用 / Active NIC Tracking & Zero-Registry**: OS ルートおよび通信量に応じたアクティブ NIC 自動追従（IPv4/CIDR・サブネット・GW・DNS表示）、各行ワンクリックコピー／全情報一括コピー、Windows レジストリを一切使わない自動起動切替（`SimpleStats.lnk`）、OS 言語に応じた英語／日本語自動切替に対応。
    *   Automatically tracks the active network adapter, supports 1-click row & full-report clipboard copy, zero-registry Windows startup toggle, and automatic English / Japanese UI localization.

## 動作環境 / System Requirements

*   **OS**: Windows 10 / Windows 11 (x64)
*   **構成 / Distribution**: 単一の実行ファイル（`SimpleStats.exe`）。追加の .NET ランタイムやインストーラーは不要です / Standalone single-file executable; no separate .NET runtime installation required.

## 利用規約 / Terms of Use

*   **ライセンス / License**: フリーウェア（個人・法人問わず無料） / Freeware (free for personal and commercial use).
*   **著作権 / Copyright**: chilili kobo に帰属します / Belongs to chilili kobo.
*   **免責 / Disclaimer**: 本ソフトウェアは「現状有姿（As-Is）」で提供され、使用による損害について作者は一切の責任を負いません / Provided "As-Is" without warranty; the author assumes no liability for any damages.

## クレジット / Credits (Open-Source Notices)

This application is built with the .NET NativeAOT runtime and native Windows APIs, without third-party UI packages. For copyright notices and license details, refer to [ThirdPartyNotices.md](ThirdPartyNotices.md).

本ソフトウェアはサードパーティ製UIライブラリを使用せず、.NET NativeAOT ランタイムおよび Windows 標準 API のみで構築されています。ランタイムの著作権表示およびライセンス条文は [ThirdPartyNotices.md](ThirdPartyNotices.md) をご参照ください。

---

**Author**: chilili kobo  
**Product Page (JP)**: [https://chililikobo.github.io/simple-stats.html](https://chililikobo.github.io/simple-stats.html)  
**Product Page (EN)**: [https://chililikobo.github.io/en/simple-stats.html](https://chililikobo.github.io/en/simple-stats.html)  
**X (Twitter)**: [@chililikobo](https://x.com/chililikobo)
