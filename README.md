# 2020 教育部全國大專校院人工智慧競賽 (AI CUP) - 機器閱讀紀錄-課程挑戰賽
## 主辦單位：[T-Brain 網站](https://tbrain.trendmicro.com.tw/Competitions/Details/12)
## 競賽摘要
- 隊伍名稱：StarRingChild
- 參賽成績：第 3 名 / 共 148 組參賽隊伍
- 競賽任務：從 arXiv 的電腦科學相關論文摘要，預測出摘要所屬的類別

## 專案描述
本競賽實質上是練習賽，參賽單純是要讓自己熟悉 [HuggingFace-transformers](https://github.com/huggingface/transformers) 的 Tokenizer 與 Embedding 使用方法。

程式碼與模型架構皆引用自 2019 年相關賽事之 [冠軍隊伍](https://github.com/steven95421/AI-CUP-2019-task2)，我做的修改只有 2020 年隨著新的套件更新與 debug ，例如：
- GELU 從自定義函數改成 PyTorch 內的 torch.nn.GELU
- transformers 的 WarmupLinearSchedule 改成 get_linear_schedule_with_warmup
