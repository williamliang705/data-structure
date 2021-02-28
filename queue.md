# Queue 佇列

## 介紹

Queue 是具有 First-in-first-out(FIFO) 特性的資料結構，先進入 queue 中的元素，會先被移除。

舉例來說就像是排隊買電影票，先進入排隊隊伍(queue)的人可以先買到票並優先離開，而後到的必須等到前面的人買完才能輪到他。

## 如何實作?

首先我們需要一個 array 表示 queue 和一個指標表示 head 位置，當有元素移出時，或是當 queue 為空並有新元素加入時，都會改變 head 指向的位置。

![img](https://s3-lc-upload.s3.amazonaws.com/uploads/2018/07/21/screen-shot-2018-07-21-at-153558.png)

![img](https://s3-lc-upload.s3.amazonaws.com/uploads/2018/07/21/screen-shot-2018-07-21-at-153713.png)

但這種方式會隨著 head 的移動，會有越來越多的空間被浪費，於是衍生出另一種 queue，稱為 **Circular Queue**

