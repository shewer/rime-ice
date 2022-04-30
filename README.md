# 自用 Rime 配置

![demo](./demo.jpg)



## 基本套路：

-   简体、全拼
    - 鼠须管 Squirrel 0.15.2 
    - 小狼毫 Weasel 0.14.3
-   「[袖珍简化字方案](https://github.com/rime/rime-pinyin-simp)」作为基础
    - [简繁切换](https://github.com/rime/home/issues/388#issuecomment-504572224)
    - [动态日期、时间、星期](https://github.com/KyleBing/rime-wubi86-jidian)
    - 所有标点符号直接上屏，「/」模式改为「v」模式，「/」直接上屏
    - 将「[Emoji](https://github.com/rime/rime-emoji)」改为词语与符号映射
    - 增加了许多拼音纠错
-   融合「[melt_eng](https://github.com/tumuyan/rime-melt)」英文输入方案和词库
-   纯简体字表、词库（这样在用户词典中也是简体了）
    - 字表：[《通用规范汉字表》的 8105 字字表](https://github.com/iDvel/The-Table-of-General-Standard-Chinese-Characters)
    - 词库：「[华宇野风系统词库](http://bbs.pinyin.thunisoft.com/forum.php?mod=viewthread&tid=30049)」 +「[清华大学开源词库](https://github.com/thunlp/THUOCL)」
    - 「[简体八股文语言模型](https://github.com/lotem/rime-octagram-data/tree/hans)」

<br>

**请先将 `pinyin_simp.dict.yaml` 中的  `- cn_dicts/private` 这行删除，这是我自己的私人词库（联系人之类的），否则鼠须管无法部署，小狼毫只能输入英文。**

<br>

详细介绍：[我的 Rime 配置 2022](https://dvel.me/posts/my-rime-setting-2022/)
