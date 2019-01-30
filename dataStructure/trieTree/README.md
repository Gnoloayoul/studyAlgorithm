# 字典树
算法描述：trie树的本质，就是利用字符串之间的公共前缀，将重复的前缀合并在一起。
时间复杂度：构建O(n)，查询O(k)
## 算法步骤
* 根节点/ 什么都不表示
* 做一个字典比如a-z 字母表
* 没一个节点包含这26个字母的字典表，每个位置保存下个节点的指针。
## 算法分析
缺点：
* trie树比较消耗内存：因为他没一层都保存一个字典表，就算这层的节点只有一个也要有一组表
* 使用的是指针类型，内存不连续对存储不友好，性能打折扣
优点：
* 查询效率比较高，对于一些范围较小的或者内存不敏感的应用可以使用
* 特别适用自动补全类应用