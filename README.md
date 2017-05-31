警察局分佈與案發地區分析
================

B0144201戴維政 B0444228林鈺潔

作業說明 （繳交時請直接刪除這個章節）
-------------------------------------

作業目的：期末專題暖身

依下列指示，完成期末分析專題作業規劃：

-   訂出分析問題，並將R Markdown的一級標題(第一行的title:)中的"長庚大學 大數據分析方法 作業六"取代為期末專題的分析問題，並在分析議題背景前加上組員姓名 (`10pt`)
-   分析議題背景 (`10pt`) 與動機 (`10pt`)
-   資料說明 (`10pt`) 與 載入 (`10pt`)
-   資料處理與清洗 (`10pt`) 說明 (`10pt`)
-   對資料們進行探索式資料分析，圖文並茂佳!(`20pt`)
-   期末專題分析規劃與假設 (`10pt`)

分析議題背景
------------

在風聲鶴唳，草木皆兵的社會中，走在路上都有可能被砍，犯罪層出不窮。 \#\# 分析動機 總是在新聞上看到令人無法想像的行為，警察的存在對罪犯而言似乎毫無威脅，因此想分析各地區派出所的數量是否會影響犯罪的數量，進一步探討警力的強度和存在的必要性。 \#\# 使用資料 派出所的所在地點以及近兩年的犯罪分佈地點

``` r
library(readr)
```

    ## Warning: package 'readr' was built under R version 3.2.5

``` r
policeS <- read_csv("~/Downloads/mapdata201705260605/policeS.csv")
```

    ## Parsed with column specification:
    ## cols(
    ##   中文單位名稱 = col_character(),
    ##   英文單位名稱 = col_character(),
    ##   郵遞區號 = col_integer(),
    ##   地址 = col_character(),
    ##   電話 = col_character(),
    ##   POINT_X = col_double(),
    ##   POINT_Y = col_double()
    ## )

``` r
X10401_10403犯罪資料 <- read_csv("~/Downloads/10401-10403犯罪資料.csv") 
```

    ## Parsed with column specification:
    ## cols(
    ##   案類 = col_character(),
    ##   發生日期 = col_integer(),
    ##   發生地點 = col_character()
    ## )

``` r
X10404_10406犯罪資料 <- read_csv("~/Downloads/10404-10406犯罪資料.csv") 
```

    ## Warning: Missing column names filled in: 'X4' [4]

    ## Parsed with column specification:
    ## cols(
    ##   案類 = col_character(),
    ##   發生日期 = col_integer(),
    ##   發生地點 = col_character(),
    ##   X4 = col_character()
    ## )

``` r
X10407_10409犯罪資料 <- read_csv("~/Downloads/10407-10409犯罪資料.csv") 
```

    ## Warning: Missing column names filled in: 'X4' [4]

    ## Parsed with column specification:
    ## cols(
    ##   案類 = col_character(),
    ##   發生日期 = col_integer(),
    ##   發生地點 = col_character(),
    ##   X4 = col_character()
    ## )

``` r
X10410_10412犯罪資料 <- read_csv("~/Downloads/10410-10412犯罪資料.csv") 
```

    ## Warning: Missing column names filled in: 'X4' [4]

    ## Parsed with column specification:
    ## cols(
    ##   案類 = col_character(),
    ##   發生日期 = col_integer(),
    ##   發生地點 = col_character(),
    ##   X4 = col_character()
    ## )

``` r
X10501_10503犯罪資料 <- read_csv("~/Downloads/10501-10503犯罪資料.csv")
```

    ## Warning: Missing column names filled in: 'X4' [4]

    ## Parsed with column specification:
    ## cols(
    ##   案類 = col_character(),
    ##   發生日期 = col_integer(),
    ##   發生地點 = col_character(),
    ##   X4 = col_character()
    ## )

``` r
X10504_10506犯罪資料 <- read_csv("~/Downloads/10504-10506犯罪資料.csv")
```

    ## Warning: Missing column names filled in: 'X4' [4]

    ## Parsed with column specification:
    ## cols(
    ##   案類 = col_character(),
    ##   發生日期 = col_integer(),
    ##   發生地點 = col_character(),
    ##   X4 = col_character()
    ## )

``` r
X10507_10509犯罪資料 <- read_csv("~/Downloads/10507-10509犯罪資料.csv")
```

    ## Warning: Missing column names filled in: 'X4' [4]

    ## Parsed with column specification:
    ## cols(
    ##   案類 = col_character(),
    ##   發生日期 = col_integer(),
    ##   發生地點 = col_character(),
    ##   X4 = col_character()
    ## )

``` r
X10510_10512犯罪資料 <- read_csv("~/Downloads/10510-10512犯罪資料.csv")
```

    ## Warning: Missing column names filled in: 'X4' [4]

    ## Parsed with column specification:
    ## cols(
    ##   案類 = col_character(),
    ##   發生日期 = col_integer(),
    ##   發生地點 = col_character(),
    ##   X4 = col_character()
    ## )

資料處理與清洗
--------------

將近兩年的犯罪資料以地區做合併 再以犯罪資料的發生地區和派出所清理後的地址做合併

``` r
#這是R Code Chunk
```

探索式資料分析
--------------

圖文並茂圖文並茂

``` r
#這是R Code Chunk
```

期末專題分析規劃
----------------

期末專題要做XXOOO交叉分析
