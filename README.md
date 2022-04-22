# must-know-r-tricks
- Search an object (function, variabl, etc.) in a specified folder (can also go to Edit -> Find in Files): keyboard shortcuts: ctrl + shift + F
- Shortcut for %>%: ctrl + shift + M
- To view the data frame in the data manipulation, just add %>% View() to the end. 
- calculate rolling sum by default
https://stackoverflow.com/questions/63662697/calculate-rolling-sum-by-group
- common scripts/functions:
getwd(): check current working directory
- Comment multiple lines: Ctrl + Shift + C
- Pattern matching looks for a given pattern in data
  x <- c(“d”, “a”, “c”, “abba”)
  grepl(“a”, x)
  [1] FALSE  TRUE FALSE  TRUE

  x <- c(“d”, “a”, “c”, “abba”)
  grep(“a”, x)
  [1] 2 4


  pattern <- “ab[0-9]”
  strings <- c(‘ab9’, ‘ab’, ‘abc8’, ‘abc’, ‘ab1’)
  print (grepl(pattern, strings))
