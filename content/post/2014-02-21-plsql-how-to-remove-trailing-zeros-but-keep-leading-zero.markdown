---
author: ewmanning
comments: true
date: 2014-02-21 11:49:59+00:00
layout: post
link: https://edwardmanning.wordpress.com/2014/02/21/plsql-how-to-remove-trailing-zeros-but-keep-leading-zero/
slug: plsql-how-to-remove-trailing-zeros-but-keep-leading-zero
title: PL/SQL - How to Remove Trailing Zeros but Keep Leading Zero
wordpress_id: 141
categories:
- Wiki
tags:
- Formatting
- Oracle
- PL/SQL
---

WITH T AS 
    (
      SELECT 100 AS EXAMPLE FROM DUAL
      UNION 
      SELECT 98.336 AS EXAMPLE FROM DUAL
      UNION
      SELECT 25 AS EXAMPLE FROM DUAL
    )
    
    SELECT 
      EXAMPLE / 100 AS EXAMPLE_1,
      TO_CHAR(EXAMPLE / 100) AS EXAMPLE_2,
      RTRIM(TO_CHAR(EXAMPLE / 100, 'FM0.999999999999'), '.') AS EXAMPLE_3
    FROM T;


![PL/SQL leading zero with no trailing zeros](/static/2014/02/plsql-leading-trailing-zeros.png)





Thanks to [Oracle Community](https://community.oracle.com/message/9625400)
