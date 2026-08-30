---
title: 算法笔记本
published: 2026-08-30
description: "林国坚的笔记本1"
draft: false
---

胜 负 已 分

## 随手记

lower_bound：第一个 ≥ L 的位置（第一个不小于 L 的）
upper_bound：第一个 > L 的位置（第一个严格大于 L 的）
upper_bound(a.begin(), a.end(), L) 在已经排好序的区间里，返回第一个严格大于 L 的元素的迭代器（一个"指针"）。
a.end() - upper_bound(a.begin(), a.end(), L)
a.end() 指向数组末尾（最后一个元素后面一格），用它减去"第一个大于 L 的位置"，得到的差就是大于 L 的元素个数。
两个函数都是二分查找，复杂度 O(log n)。

## 技巧

## 题目

## 模板

## Markdown格式速查

### 1. 标题（分区用）

井号越多，标题越小；标题会自动生成目录锚点。

```markdown
## 技巧          ← 二级标题（大分区）
### lower_bound  ← 三级标题（具体知识点）
```

### 2. 加粗

用 `**` 包起来：

```markdown
**第一个 ≥ L 的位置**
```

### 3. 行内代码

用反引号 `` ` `` 包起来（键盘左上角 Esc 下面那个键）：

```markdown
`lower_bound` 复杂度 `O(log n)`
```

### 4. 代码块

三个反引号 + 语言名（自动高亮 + 行号）：

````markdown
```cpp
auto it = upper_bound(a.begin(), a.end(), L);
int cnt = a.end() - it;
```
5. 列表

- 第一点
- 第二点
6. 数学公式（KaTeX）
行内：$O(\log n)$　独立：$$a_{n+1} = a_n + d$$

例子：lower_bound 与 upper_bound
lower_bound：第一个 ≥ L 的位置（第一个不小于 L 的）
upper_bound：第一个 > L 的位置（第一个严格大于 L 的）

upper_bound(a.begin(), a.end(), L)
// 返回第一个严格大于 L 的元素的迭代器（一个"指针"）
int cnt = a.end() - upper_bound(a.begin(), a.end(), L);
// a.end() 指向数组末尾，减去"第一个大于 L 的位置"，得到大于 L 的元素个数
两个函数都是二分查找，复杂度 $O(\log n)$。



---