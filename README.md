# CRF-
自然语言处理之CRF条件随机场
<br>
还没有进行整理，大致就是通过利用中文停用词表和已有词表结合最大逆向匹配算法进行打标签操作，分成10 份，乱序，
<br>
计算加权调和平均数，概率如果大于0.90，则表示成功，否则改变分词策略，如果成功，取十份当中F
<br>
值最大的MODEL，将大量原始文本用(。!;?) 分句完，让机器直接根据model 去学习，然后根据
<br>
生成的标签文本进行逆向处理，将文本还原成斜杠分割的样子.