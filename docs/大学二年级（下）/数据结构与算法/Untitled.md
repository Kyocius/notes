# 第六章作业

吴优 2023212716

## 第一题

![image-20250516222350633](C:\Users\kyoci\AppData\Roaming\Typora\typora-user-images\image-20250516222350633.png)

## 第二题

```c
bool Similar(BiTree p, BiTree q) {
    if (!p && !q) return true; // 都为空，结构相同
    if (!p || !q) return false; // 一个为空，一个不为空
    return Similar(p->lc, q->lc) && Similar(p->rc, q->rc); // 递归判断左右子树
}
```

## 第三题

```c
#include <stdbool.h>
#include <stdlib.h>
bool JudgeComplete(BiTree root) {
    if (!root) return true;
    BiTree queue[1000];
    int front = 0, rear = 0;
    bool mustBeLeaf = false;
    queue[rear++] = root;
    while (front < rear) {
        BiTree node = queue[front++];
        if (node->lc) {
            if (mustBeLeaf) return false;
            queue[rear++] = node->lc;
        } else {
            mustBeLeaf = true;
        }
        if (node->rc) {
            if (mustBeLeaf) return false;
            queue[rear++] = node->rc;
        } else {
            mustBeLeaf = true;
        }
    }
    return true;
}
```

## 第四题

```c
int countChildren(CSTree node) {
    int count = 0;
    CSTree p = node->firstchild;
    while (p) {
        count++;
        p = p->nextsibling;
    }
    return count;
}
int degree(CSTree root) {
    if (!root) return 0;
    int maxDeg = countChildren(root);
    for (CSTree child = root->firstchild; child; child = child->nextsibling) {
        int childDeg = degree(child);
        if (childDeg > maxDeg) maxDeg = childDeg;
    }
    return maxDeg;
}
```

## 第五题

```c
int Count(CSTree root) {
    if (!root) return 0;
    if (!root->firstchild) return 1; // 没有孩子，是叶子
    int count = 0;
    for (CSTree child = root->firstchild; child; child = child->nextsibling) {
        count += Count(child);
    }
    return count;
}
```

## 第六题

![image-20250516222539330](C:\Users\kyoci\AppData\Roaming\Typora\typora-user-images\image-20250516222539330.png)

![image-20250516222551399](C:\Users\kyoci\AppData\Roaming\Typora\typora-user-images\image-20250516222551399.png)

## 第七题

若树为空：⽆叶⼦，命题成⽴。

若树只有1个叶⼦：三种遍历都只包含这个叶⼦，顺序相同。

若有多个叶⼦，由于遍历⽅式虽然对⾮叶节点顺序有差异，但都遵循左⼦树优先于右⼦树的结构规则，⽽叶⼦本⾝⼜不再包含其他⼦结构，故相对位置不变。

## 第八题

![image-20250516222706765](C:\Users\kyoci\AppData\Roaming\Typora\typora-user-images\image-20250516222706765.png)

## 第十题

![image-20250517001118291](C:\Users\kyoci\AppData\Roaming\Typora\typora-user-images\image-20250517001118291.png)