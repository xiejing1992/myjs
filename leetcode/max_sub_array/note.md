##关于动态规划的一些记录

####通常我们遍历子串或者子序列有三种方式
示例[a,b c, d]
 * 以某个节点为开头的所有字串或者序列: 如[a], [a,b], [a,b,c] .....再从b开始重新遍历
 * 根据子序列或者子串的长度为标准，先遍历出长度为1的子串，再遍历出长度为2的子串
 * 以子序列的结束点位基准，先遍历出以某个节点为结束点的所有子序列，因为每个点都可能为子序列的结束点，因此要遍历下整个序列如: 以 b 为结束点的所有子序列: [a , b], [b] 以 c 为结束点的所有子序列: [a, b, c], [b, c], [ c ]。
第三种遍历，因为可以产生递推的关系，采用动态规划时，通常可以使用此种遍历方式， 
刚接触动态规划时，需要熟悉第三种遍历方式是 核心



