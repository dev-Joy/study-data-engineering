### RDD (Resilient Distributed Dataset)

: 복구 가능한 분산 데이터세트

### function

- reduceByKey()
  : combine values with the same key using some function.
- groupByKey()
  : Group values with the same key
- sortByKey()
  : Sort RDD by key values
  > your transformation doesn't affect the keys.
- mapValues()
  : 1:1
- flatMapValues()
  : N:1
