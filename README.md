## 群益證券 API 非官方範例

### 重點提示

群益 API 元件是採用 Visual C++ 2010 開發，並且封裝標準函式庫採用動態連結，  
因此若 Windows 缺少 Visual Studio 2010 可轉發套件，註冊元件時就會發生錯誤，  
在一台乾淨的 Windows 上照著[官方影片](https://www.youtube.com/watch?v=OgNjvXuBaoI)教學操作，肯定是會卡關的。

### 使用環境安裝範例
```
(base) PS>python setup.py
安裝 Visual C++ 2010 可轉發套件
Visual C++ 2010 可轉發套件已安裝, 版本: 10.0.40219.325
安裝與註冊群益 API 元件
群益 API 元件已安裝, 版本: 2.13.16.0
```

### 使用 Ticks 監聽範例

```
(base) PS>python ticks.py
登入成功
連線成功
連線就緒
產品資訊載入完成
[0050 元大台灣50] 時間:13:30:00.000 買:82.55 賣:82.50 成:82.55 單量:476 總量:13554
...
```

### 使用日 K 監聽範例

```
(base) PS>python kline.py
登入成功
連線成功
連線就緒
產品資訊載入完成
[0050 元大台灣50] 日期:2003-06-30 開:37.10 收:37.08 高:37.40 低:36.92 量:9930
[0050 元大台灣50] 日期:2003-07-01 開:37.09 收:38.05 高:38.10 低:37.09 量:14290
[0050 元大台灣50] 日期:2003-07-02 開:38.17 收:38.69 高:38.82 低:38.10 量:16232
[0050 元大台灣50] 日期:2003-07-03 開:40.60 收:39.00 高:40.60 低:38.81 量:16839
[0050 元大台灣50] 日期:2003-07-04 開:39.10 收:39.26 高:39.26 低:38.75 量:12491
...
```

### 金管會相關規定
* [修正「電子票證應用安全強度準則」](http://law.fsc.gov.tw/law/NewsContent.aspx?id=6292)
* [有關證券暨期貨市場各服務事業建立內部控制制度處理準則第三十六條之二及第三十七條規定之令](http://law.fsc.gov.tw/law/LawContent.aspx?id=GL002440)
