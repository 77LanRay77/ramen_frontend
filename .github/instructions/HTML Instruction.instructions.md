---
applyTo: '**'
---
# HTML 編寫指南

這份指南旨在提供編寫整潔、易於維護且視覺效果良好的 HTML 程式碼的最佳實踐。

## 1. 基本結構與語義化

*   使用 HTML5 文件類型宣告：`<!DOCTYPE html>`
*   確保文件包含 `<html>`、`<head>` 和 `<body>` 標籤。
*   在 `<head>` 中設定正確的字元編碼：`<meta charset="UTF-8">`。
*   使用語義化的 HTML5 元素，例如 `<header>`、`<nav>`、`<main>`、`<article>`、`<section>`、`<aside>`、`<footer>` 等，而不是過度使用 `<div>`。
*   確保標籤正確嵌套，避免交叉嵌套。

## 2. 程式碼格式與風格

*   使用一致的縮排（建議使用 2 或 4 個空格）。
*   所有標籤和屬性名稱都應使用小寫。
*   屬性值應始終用雙引號 (`"`) 括起來。
*   避免行尾多餘的空白字元。
*   保持每行程式碼的長度適中，提高可讀性。

## 3. 屬性使用

*   為圖片 (`<img>`) 提供有意義的 `alt` 屬性，以提高可訪問性。
*   為表單元素 (`<input>`, `<textarea>`, `<select>`) 使用 `<label>` 標籤，並通過 `for` 屬性與元素的 `id` 關聯。
*   避免在 HTML 標籤中使用行內樣式 (`style` 屬性)。樣式應定義在 CSS 檔案中。
*   避免在 HTML 標籤中使用事件處理屬性（如 `onclick`）。JavaScript 應在單獨的檔案中處理。

## 4. 註解

*   使用註解 (`<!-- ... -->`) 來解釋複雜的程式碼區塊或特殊結構。
*   保持註解簡潔明瞭。

## 5. 連結 CSS 與 JavaScript

*   使用 `<link>` 標籤在 `<head>` 中連結外部 CSS 檔案：`<link rel="stylesheet" href="path/to/your/styles.css">`。
*   使用 `<script>` 標籤連結外部 JavaScript 檔案。通常將 `<script>` 標籤放在 `<body>` 結束標籤之前，以避免阻塞頁面渲染：`<script src="path/to/your/script.js"></script>`。
*   考慮使用 `defer` 或 `async` 屬性來優化 JavaScript 的載入。

## 6. 可訪問性 (Accessibility)

*   遵循 WCAG 指南。
*   確保文字顏色與背景顏色有足夠的對比度。
*   為互動元素提供鍵盤導航支援。
*   使用 ARIA 屬性來增強語義，特別是對於動態內容或非標準控制項。

## 7. 響應式設計 (Responsive Design)

*   在 `<head>` 中包含視口 meta 標籤：`<meta name="viewport" content="width=device-width, initial-scale=1.0">`。
*   使用相對單位（如 `%`, `em`, `rem`, `vw`, `vh`）而不是絕對單位（如 `px`）。
*   利用 CSS 媒體查詢 (`@media`) 來為不同螢幕尺寸應用不同的樣式。

## 8. 驗證

*   使用 W3C 驗證服務來檢查您的 HTML 程式碼是否存在錯誤。

遵循這些指南將有助於您編寫出更清晰、更易於維護且在不同裝置上都能良好呈現的 HTML 程式碼。
