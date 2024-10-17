# 原始版本ASC_IP_LRU

# 執行程式
- python run.py
- 輸入cache_size(0.5% : 21990232555)
- 選擇使用的policy 輸入0或1
- 選擇使用的trace 輸入0

# 程式結構
- run.py : 主程式，負責設定trace,policy,cache_size
- ASC_IP_LECAR.py : 引用ASC_IP.py並且將LRU部分改用ASC_IP_LRU
- ASC_IP_LRU.py : 繼承ASC_IP.py，改寫部分只有增加統計debug資訊的部分
- lib/ASC_IP.py : 完整ASC_IP_LRU功能，會被引用來實現 ASC_IP_LRU和ASC_IP_LECAR


# TRACE
trace下載網址:https://drive.google.com/file/d/17lv8Zd6DG1TyBdJw1WlGV25heeicDuYp/view?usp=sharing

trace位置 "D:/all_Trace/ASC-IP/wiki2018"

trace格式 : 每一行是一個request，且每行內容為 id , size

註:原始格式為 : 每一行是一個request，且每行內容為 time , id , size , extra_feature
原始版本網址 : https://github.com/sunnyszy/lrb
