---
title: Understand that CROSS JOIN UNNEST works through value tables
title-cs: CROSS JOIN UNNEST funguje kvůli tvorbě value tables
category: data-coding
tags: [idea, sql]
season: winter
created: 06 Jun 2020
updated: 05 Jan 2022
sources: https://stackoverflow.com/questions/47670451/sql-array-flattening-why-doesnt-cross-join-unnest-join-every-nested-value-with
---

Now let's talk about unnesting.

The `UNNEST` function takes an array and returns a value table of the array's element type. Whereas most BigQuery tables are SQL tables defined as a collection of columns, a value table has rows of some value type.

For `numbers_array`, `UNNEST(numbers_array)` returns a value table whose value type is `INT64`, since `numbers_array` is an array with an element type of `INT64`. This value table contains all of the elements in `numbers_array` for the current row from `t1`