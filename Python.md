# DataAnalysisTool

## 目錄
- [簡介](#簡介)
- [功能](#功能)
- [安裝](#安裝)
- [使用方法](#使用方法)
- [貢獻](#貢獻)
- [授權](#授權)

## 簡介
DataAnalysisTool 是一個用於數據清洗和分析的 Python 工具，旨在簡化數據處理流程。

## 功能
- 數據清洗：去除缺失值、重複值
- 數據分析：統計描述、可視化
- 數據導出：支持多種格式

## 安裝

### 前提條件
- Python 版本 3.8 或更高

### 安裝步驟
1. 克隆此存儲庫
    ```bash
    git clone https://github.com/username/DataAnalysisTool.git
    ```
2. 進入專案目錄
    ```bash
    cd DataAnalysisTool
    ```
3. 創建虛擬環境並激活
    ```bash
    python -m venv venv
    source venv/bin/activate  # 對於 Windows，使用 `venv\Scripts\activate`
    ```
4. 安裝依賴
    ```bash
    pip install -r requirements.txt
    ```

## 使用方法
1. 導入模塊
    ```python
    from data_analysis_tool import DataCleaner, DataAnalyzer
    ```
2. 加載數據
    ```python
    data = pd.read_csv('your_data.csv')
    ```
3. 清洗數據
    ```python
    cleaner = DataCleaner(data)
    cleaned_data = cleaner.clean()
    ```
4. 分析數據
    ```python
    analyzer = DataAnalyzer(cleaned_data)
    summary = analyzer.summarize()
    analyzer.plot_histogram('column_name')
    ```

## 貢獻
歡迎貢獻！請閱讀 [CONTRIBUTING.md](CONTRIBUTING.md) 了解詳細信息。

## 授權
此專案基於 [MIT 授權](LICENSE)。
