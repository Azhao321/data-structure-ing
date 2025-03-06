# 二叉树
二叉树的遍历方式：前序、中序、后序、层序

# C++ vector与list插入的不同点：
## vector：
vector插入时从原理上来说是复制当前数组扩容，从而进行插入 <br>
插入格式是直接点明位置 <br>
eg: <br>
vec.insert(vec.begin() + i ，插入内容)//i就是插入的位置
## list
list是链表，可以直接改变指针的前后节点，因此是针对指针的操作，插入时不能点名位置，需要使用迭代器 <br>
eg: <br>
std::list<int>::iterator it = list.begin(); <br>
//简便写法：auto it = list.begin(); <br>
插入位置，可以使用it++，加多少根据具体实例迭代； <br>
list.insert(it, 插入内容)<br>
