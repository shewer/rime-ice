# 自用 Rime 配置

![demo](./demo.jpeg)



## 基本套路：

-   简体全拼
    - 鼠须管 Squirrel 0.15.2 
    - 小狼毫 Weasel 0.14.3
-   「[袖珍简化字方案](https://github.com/rime/rime-pinyin-simp)」作为基础
    - [简繁切换](https://github.com/rime/home/issues/388#issuecomment-504572224)
    - [日期、时间、星期](https://github.com/KyleBing/rime-wubi86-jidian)
    - [以词定字](https://github.com/BlindingDark/rime-lua-select-character)
    - [长词优先](https://github.com/tumuyan/rime-melt/blob/master/lua/melt.lua)
    - 所有标点符号直接上屏，「/」模式改为「v」模式，「/」直接上屏
    - 将「[Emoji](https://github.com/rime/rime-emoji)」改为词语与符号映射
    - 增加了许多拼音纠错
-   融合「[melt_eng](https://github.com/tumuyan/rime-melt)」英文输入方案和词库
    -   [优化英文输入体验](https://dvel.me/posts/make-rime-en-better/)
-   纯简体字表、词库
    -   [《通用规范汉字表》的 8105 字字表](https://github.com/iDvel/The-Table-of-General-Standard-Chinese-Characters)
    -   [华宇野风系统词库](http://bbs.pinyin.thunisoft.com/forum.php?mod=viewthread&tid=30049)
    -   [现代汉语常用词表](https://gist.github.com/indiejoseph/eae09c673460aa0b56db)
    -   [简化字八股文](https://github.com/rime/rime-essay-simp)
    -   [清华大学开源词库](https://github.com/thunlp/THUOCL)
    -   [中文维基词库](https://github.com/felixonmars/fcitx5-pinyin-zhwiki)
    -   [八股文语言模型](https://github.com/lotem/rime-octagram-data/tree/hans)
-   长期修订词库
    -   修正大量错字、错音、异形词
    -   校对大量词汇，主要参考[校对网](http://www.jiaodui.com/bbs/)


<br>

**请先将 `pinyin_simp.dict.yaml` 中的  `- cn_dicts/private` 这行删除，这是我自己的私人词库（联系人之类的），否则鼠须管无法部署，小狼毫只能输入英文。**

<br>

详细介绍：[我的 Rime 配置 2022](https://dvel.me/posts/my-rime-setting-2022/)
