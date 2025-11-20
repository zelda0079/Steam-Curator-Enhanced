

# 📘 Steam Curator Enhanced

### *(Tampermonkey Userscript)*

### **Updated for Version 1.1**

---

# 🇺🇸 English Version

![sample](https://raw.githubusercontent.com/zelda0079/Steam-Curator-Enhanced/refs/heads/main/sample.png)

[My Curator](https://store.steampowered.com/curator/33923354)

---

## Overview

This Tampermonkey userscript enhances the Steam Curator admin interface — including both the **Accepted Games** page and the **Stats** page.
It provides UI improvements, filtering options, language switching, stable dynamic content detection, and import/export features.

Version **1.1** includes major enhancements to navigation monitoring, dropdown behavior, multi-language support, and a *new set of features* for the **Stats** page.

---

## Features

### ✔ Accepted Page Enhancements

* **Checkboxes for each game** (persistent using localStorage)
* **Visibility Filters**

  * Show All Games
  * Show Hidden Games (checked)
  * Show Unhidden Games (unchecked)
* **Review Status Filters**

  * Reviewed & Unreviewed
  * Reviewed Only
  * Unreviewed Only
* **Bulk Actions**

  * Select All / Deselect All
* **Import / Export** checkbox states as JSON
* **Full Language Support**

  * English
  * Traditional Chinese
  * Simplified Chinese
* **Automatic Saving**
* **AJAX Detection / MutationObserver**
* **Stability Patch**

  * 100% reliable control bar rendering
  * Dropdown fixes
  * Robust dynamic page monitoring
  * Full pushState / replaceState support

---

### ✔ Stats Page Enhancements (NEW in v1.1)

* Auto-detect curator ID
* Fetch & cache Steam Community group name
* Rewrite app links to the curator’s community curation page

  * `https://steamcommunity.com/groups/<group>/curation/app/<appId>`
* Popup notifications
* High-efficiency MutationObserver for dynamic updates

---

## Installation

1. Install **Tampermonkey**
   [https://www.tampermonkey.net/](https://www.tampermonkey.net/)

2. Install the userscript:
   [https://github.com/zelda0079/Steam-Curator-Enhanced/raw/refs/heads/main/Steam_Curator_Game_Manager.user.js](https://github.com/zelda0079/Steam-Curator-Enhanced/raw/refs/heads/main/Steam_Curator_Game_Manager.user.js)

---

# 📌 CHANGELOG – Version **1.1**

### 🔧 Core System Improvements

* Reworked URL monitoring (`pushState`, `replaceState`, `popstate`)
* Added idle monitoring for `/admin/accepted` and `/admin/stats`
* Fixed initialization issues with AJAX-loaded content

---

### 🖼 Accepted Page Improvements

* Ensured control bar always loads correctly
* Dropdown stability fixes
* Better handling for dynamically added game blocks

---

### 🌐 Language System (NEW)

* Added language switcher

  * English
  * Traditional Chinese
  * Simplified Chinese
* Saved via `localStorage`

---

### 📊 Stats Page (MAJOR NEW FEATURE)

* Detect curator ID
* Fetch + cache group name
* Rewrite all app links
* Popup notifications
* Efficient MutationObserver integration

---

### 🧰 Code Structure Improvements

* Unified element detection
* Added initialization locking
* General stability improvements

---

<br>

# 🇹🇼 繁體中文版本

---

![截圖](https://raw.githubusercontent.com/zelda0079/Steam-Curator-Enhanced/refs/heads/main/sample.png)

[我的鑑賞家](https://store.steampowered.com/curator/33923354)

## 概述

此 Tampermonkey 腳本可強化 Steam 館主後台的 **已接受遊戲頁面** 以及 **統計頁面（stats）**。
提供遊戲過濾、自動儲存、批次操作、語言切換、匯入匯出、AJAX 偵測等功能。

**v1.1** 增加更穩定的 Steam 後台導航偵測、下拉式選單修復、新語言系統，以及全新的「統計頁面升級功能」。

---

## 功能

### ✔ 已接受遊戲頁面強化

* **每個遊戲方塊自動加入打勾框**
* **顯示過濾器**

  * 顯示全部
  * 顯示隱藏
  * 顯示未隱藏
* **評論狀態過濾器**

  * 已評論 + 未評論
  * 僅已評論
  * 僅未評論
* **批次操作：全選 / 取消全選**
* **匯入/匯出 JSON**
* **語言切換（英文/繁中/簡中）**
* **自動儲存至 localStorage**
* **偵測 AJAX 更新**
* **穩定性修補**

  * 工具列 100% 出現
  * 下拉式選單不會消失
  * 更強的 MutationObserver
  * 完整 Steam 後台導航監控

---

### ✔ 統計頁面強化（v1.1 新增）

* 自動偵測館主 ID
* 自動抓取並快取社群群組名稱
* 自動將所有 `/app/<id>` 改寫為 curator curation 連結
* 彈出提示顯示替換數量
* 高效能 MutationObserver

---

## 安裝方法

1. 安裝 **Tampermonkey**
   [https://www.tampermonkey.net/](https://www.tampermonkey.net/)

2. 安裝腳本：
   [https://github.com/zelda0079/Steam-Curator-Enhanced/raw/refs/heads/main/Steam_Curator_Game_Manager.user.js](https://github.com/zelda0079/Steam-Curator-Enhanced/raw/refs/heads/main/Steam_Curator_Game_Manager.user.js)

---

# 📌 更新日誌 – **v1.1**

### 🔧 核心系統修正

* 改寫 URL 偵測系統（pushState / replaceState / popstate）
* 新增背景監控：即使不重整也能偵測頁面變化
* 更穩定的初始化流程

---

### 🖼 已接受頁面改良

* 保證工具列穩定出現
* 修復下拉式選單自動收回
* 更佳的 AJAX 動態載入支援

---

### 🌐 語系系統（全新）

* 新增語言切換（英文/繁中/簡中）
* 本地儲存語言偏好

---

### 📊 統計頁面（重大新增）

* 自動取得館主資料
* 自動改寫 APP 連結
* 彈出通知
* 高效能 DOM 監控

---

### 🧰 程式結構改進

* 初始化鎖
* 統一遊戲區塊偵測
* 提升穩定性
