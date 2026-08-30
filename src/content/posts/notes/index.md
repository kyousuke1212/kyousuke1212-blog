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
