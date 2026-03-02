# Google-Maps-Review-Analysis

# 餐廳 Google 評論情緒分析與文字雲視覺化

## 專案簡介
[cite_start]現在餐廳百百種，當我們想吃某一種類時卻不知道該選哪家 [cite: 4][cite_start]。因此本專案透過收集 Google 評論，製作文字雲及文字情感分析，以數據化的方式幫助我們做出選擇 [cite: 4]。

## 開發團隊
* [cite_start]組長：109403551 黃政皓 [cite: 2]
* [cite_start]組員：109403517 蔡皓鈞 [cite: 2]

## 專案流程與核心技術
[cite_start]本專案流程分為以下四個主要階段 [cite: 6, 7, 8, 9]：
1. [cite_start]**評論收集**：不使用 Selenium，而是觀察 Google 評論的動態載入特性，運用 `requests` 抓取內容並轉為 `json` 格式，大幅提升處理效率 [cite: 11, 12, 44, 45]。
2. [cite_start]**製作文字雲**：使用 `WordCloud` 套件結合中文字型，將評論重點（如：湯頭鮮甜、食材新鮮等）視覺化 [cite: 68, 69, 70, 86]。
3. [cite_start]**詞語分析**：利用 `SnowNLP` 進行自然語言處理，分析文字的好壞情緒（分數趨近 1 為正向，趨近 0 為負向） [cite: 96, 98, 99, 101]。
4. [cite_start]**分析結果視覺化**：將情緒分析獲得的分數轉換為 DataFrame，並透過 `pandas` 與 `matplotlib` 繪製成對長條圖，直觀比較不同店家（A shop vs. B shop）的表現 [cite: 112, 116, 118, 136, 138]。

## 使用套件
* [cite_start]`requests` [cite: 44]
* [cite_start]`json` [cite: 45]
* [cite_start]`wordcloud` [cite: 47]
* [cite_start]`snownlp` [cite: 101]
* [cite_start]`pandas` [cite: 136]
* [cite_start]`matplotlib.pyplot` [cite: 48]
