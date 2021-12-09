# 自用 Rime 配置

![demo](./demo.jpg)



## 基本套路：

-   Squirrel 0.15.2 简体 全拼
-   「[袖珍简化字方案](https://github.com/rime/rime-pinyin-simp)」作为基础
    -   [简繁切换](https://github.com/rime/home/issues/388#issuecomment-504572224)
    -   [动态日期、时间、星期](https://github.com/KyleBing/rime-wubi86-jidian)
    -   所有标点符号直接上屏，「/」模式改为「v」模式，「/」直接上屏
    -   删除了「[Emoji](https://github.com/rime/rime-emoji)」，改为词语与符号映射
    -   增加了许多拼音纠错
-   融合「[easy_en](https://github.com/BlindingDark/rime-easy-en)」英文输入方案
    -   使用了「[融合拼音](https://github.com/tumuyan/rime-pinyin-simp)」的词库和拼写规则
-   纯简体字表、词库（这样在用户词典中也是简体了）
    -   字表：[《通用规范汉字表》的 8105 字字表](https://github.com/iDvel/The-Table-of-General-Standard-Chinese-Characters)
    -   词库：「[华宇野风系统词库](http://bbs.pinyin.thunisoft.com/forum.php?mod=viewthread&tid=30049)」 +「[清华大学开源词库](https://github.com/thunlp/THUOCL)」
    -   「[简体八股文语言模型](https://github.com/lotem/rime-octagram-data/tree/hans)」
-   长期持续修订遇到的异形词、错别字、错误注音

<br>

## 说明

**部署前请先将 `pinyin_simp.dict.yaml ` 中的 `- cn_dicts/private` 这行删除，这是我自己的私人词库（联系人之类的），否则部署时会报错。**

<br>

各文件说明：

```
.
├── default.custom.yaml  # 全局设置
├── squirrel.custom.yaml # 皮肤设置

├── pinyin_simp.schema.yaml # 拼音方案（关键配置文件）
├── symbols.custom.yaml     # 自定义 symbols，单独拆分出来了，主要是将「/」模式改为了「v」模式
├── pinyin_simp.dict.yaml   # 挂载词库
├── cn_dicts/               # 词库主目录

├── easy_en.schema.yaml # 英文方案
├── easy_en.dict.yaml   # 挂载词库
├── en_dicts/           # 词库主目录

├── custom_phrase.txt # 自定义文本
├── opencc/           # Emoji、符号、词语映射
├── rime.lua          # lua 脚本
└── zh-hans-t-essay-bgw.gram # 八股文语言模型
```

<br>

将英文输入方案挂载进拼音输入方案，词库也是独立分开的。

为了完善输入体验，英文的权重设为了「0」，这会导致单编码时，候选项被大量英文占据。

为了解决这个问题，引入了 `custom_phrase.txt` 将单编码固定死，并给予高于英文方案的权重。

<br>

## 参考 & 感谢

希望本配置帮助到了你，以下是我上手时主要参考的仓库，表示感谢：

[qingmail](https://github.com/qingmail)/**[rime](https://github.com/qingmail/rime)** 详细的图文教程及实例

[fkxxyz](https://github.com/fkxxyz)/**[rime-cloverpinyin](https://github.com/fkxxyz/rime-cloverpinyin)** 四叶草拼音输入方案

[BlindingDark](https://github.com/BlindingDark)/**[rime-easy-en](https://github.com/BlindingDark/rime-easy-en)** easy_en 输入方案

[tumuyan](https://github.com/tumuyan)/**[rime-pinyin-simp](https://github.com/tumuyan/rime-pinyin-simp)** 融合拼音输入方案

[placeless](https://github.com/placeless)/**[squirrel_config](https://github.com/placeless/squirrel_config)** 见过的最酷炫的只有两个候选项的小鹤双形 

