---
title: A Small Note on Box-Cox Transformations
author: Michal Ondras
date: '2018-03-28'
categories:
  - R
slug: a-quick-note
---

If you've ever thought why a procedure doesn't exist for a process, then you like me didn't search exhaustively... enough.  Fortunately, the Box-Cox prodedure can assist in determining a data transformation or regression transformation for you -- if that's your thing.  In this note, I want to perform a transformation on my regression so that residuals are normal with a constant mean and variance. 

There are several ways to represent the tranform, but in generalities, it looks like: 

`$$Y(\lambda) = \Bigg\{\begin{array} 1\frac{Y^{\lambda}-1}{\lambda} & \text{if } \lambda \ne 0 \\ \log(Y) & \text{if } \lambda = 0 \end{array}$$`

