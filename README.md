# DBA_QueryOptimization
查詢(敘述句)最佳化

當查詢引擎接收到一條使用者查詢請求時，查詢引擎會依據該查詢敘述的類型進行 class | group 分類處理，然而在 process 查詢敘述之前，會先行考量其中 cost (代價)，即查詢敘述求解最佳『存取路徑』的成本。

有些查詢引擎會使用查詢計畫快取機制 query plans cashing | query paths caching 。 倘若使用前者，則需要注意，查詢敘述需要滿足一定條件，才能對其使用快取，否則將會導致查詢結果不正確。


