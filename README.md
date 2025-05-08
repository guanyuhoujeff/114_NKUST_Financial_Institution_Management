# 金融市場與機構研討 - 114 學年度下學期 (國立高雄科技大學)


此 GitHub 儲存庫為 **國立高雄科技大學 114 學年度下學期金融市場與機構研討(管院博士班一甲)_管院博士班一甲** 課堂作業之記錄。

## 課程資訊
- **課程名稱**: 金融市場與機構研討
- **班級**: 管院博士班一甲
- **學年度**: 114學年度下學期
- **授課教授**: 王銘駿教授
- **系所**: 金融系 - 國立高雄科技大學
- **整理人**: 侯冠宇

本專案實證分析參考陳等人(2021) 的不動產之現貨與期貨之研究。

### *Reference*
陳宜伶, 王銘駿, 詹佳縈, & 蔡己生. (2021). 間接不動產之現貨與期貨市場間的資訊傳遞—以台灣5檔營建上市股為例. *住宅學報*, 30(1), 71-101.


## Google Colab Demo
https://github.com/guanyuhoujeff/114_NKUST_Financial_Institution_Management.git

114_NKUST_Financial_Institution_Management\colab


data preprocessing : 
[檔案連結](https://github.com/guanyuhoujeff/114_NKUST_Financial_Institution_Management/tree/main/colab) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/guanyuhoujeff/114_NKUST_Financial_Institution_Management/blob/main/colab/data_preprocessing.ipynb)

VAR model : 
[檔案連結](https://github.com/guanyuhoujeff/114_NKUST_Financial_Institution_Management/tree/main/colab) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/guanyuhoujeff/114_NKUST_Financial_Institution_Management/blob/main/colab/VAR_model.ipynb)

DCC-GRACH model [open with R-Kernal] : 
[檔案連結](https://github.com/guanyuhoujeff/114_NKUST_Financial_Institution_Management/tree/main/colab) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/guanyuhoujeff/114_NKUST_Financial_Institution_Management/blob/main/colab/[r-kernal]_DCC _ARCH.ipynb)


# 在本地端運行

若想在本地端執行本系統，請依照以下步驟：

## 建置 conda 環境：
```
<!-- conda env remove -n fin-ins -y -->
conda update --all -y 
conda create -n  fin-ins  python=3.10 -y
conda activate fin-ins

conda install -c r r-irkernel -y
conda install conda-forge::r-base=4.4.3 -y
conda install -c conda-forge r-essentials  -y


pip install numpy==1.23.5 --user
pip install pandas tqdm openpyxl arch

conda install ipykernel jupyter -y
```
## 啟動 jupyter
```
conda activate fin-ins && jupyter notebook
```