# 餐廳 Google 評論情緒分析與文字雲視覺化

## 專案簡介
現在餐廳百百種，當我們想吃某一種類時卻不知道該選哪家。因此本專案透過收集 Google 評論，製作文字雲及文字情感分析，以數據化的方式幫助我們做出選擇。

## 開發團隊
* 組長：109403551 黃政皓
* 組員：109403517 蔡皓鈞

## 專案流程與核心技術
本專案流程分為以下四個主要階段：
1. **評論收集**：不使用 Selenium，而是觀察 Google 評論的動態載入特性，運用 `requests` 抓取內容並轉為 `json` 格式，大幅提升處理效率。
2. **製作文字雲**：使用 `WordCloud` 套件結合中文字型，將評論重點（如：湯頭鮮甜、食材新鮮等）視覺化。
3. **詞語分析**：利用 `SnowNLP` 進行自然語言處理，分析文字的好壞情緒（分數趨近 1 為正向，趨近 0 為負向）。
4. **分析結果視覺化**：將情緒分析獲得的分數轉換為 DataFrame，並透過 `pandas` 與 `matplotlib` 繪製成對長條圖，直觀比較不同店家（A shop vs. B shop）的表現。

## 使用套件
* `requests`
* `json`
* `wordcloud`
* `snownlp`
* `pandas`
* `matplotlib.pyplot`


## 分析結果 
**特徵文字雲**  
 <img width="349" height="181" alt="image" src="https://github.com/user-attachments/assets/8b5d8246-a35b-4ccd-9d89-685b00f5e214" />     
**留言評分分布圖**  
 <img width="387" height="278" alt="image" src="https://github.com/user-attachments/assets/59467bf0-e17d-437f-9941-41df3b146ac9" />


