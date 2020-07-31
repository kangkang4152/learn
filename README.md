# learn
平时学习经验及总结
https://www.cnblogs.com/banxian-yi/p/12365184.html


题目描述某公司需要派遣员工去国外做项目。现在，x国和y国分别需要cntx名和cnty名员工。
总经理是这样派遣员工的：每个员工有一个员工号(1,2,3……)。派遣员工总是派遣前k个员工，也即一次性派遣从1号到k号共k名员工去国外。但是，编号为x的倍数的员工不想去x国，编号为y的倍数的员工不想去y国。总经理想知道最少需要派遣前多少名员工才能满足x国和y国的需求。（也即找到最小的k，使得可以将编号为1,2,3,……k的员工分配给x国和y国，并且满足x国和y国的需求）。
解答要求时间限制：1000ms, 内存限制：64MB
输入四个整数cntx,cnty,x,y。(1<=cntx,cnty<10^9,cntx+cnty<=10^9,2<=x<y<=30000,且x和y一定是质数）
输出满足条件的最小的k。
样例输入样例 1 复制
3 1 2 3
输出样例 1
5
提示二分k，对于一个给定的k，k是满足条件的判定式是:(k-k/x>=cntx&&k-k/y>=cnty&&k-k/(x*y)>=cntx+cnty).
