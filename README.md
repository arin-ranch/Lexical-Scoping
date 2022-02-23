# Lexical-Scoping
makeCacheMatrix <- function(x = matrix()) {

}
makeVector <- function(x = numeric()) { ##define the arguement with model matrix
m <- NULL ##the value of matrix inverse
set <- function(y) { ##assign a new variable with function(y)
x <<- y ##value of matrix
m <<- NULL ##if it is a new matrix, reset value to NULL
}
get <- function() x ##assign a new variable with function(x)
setmean <- function(mean) m <<- mean ##assign a new variable with (function(mean), reset value m to mean
getmean <- function() m ## get the value of m where is called
list(set = set, get = get, ## you need this to run the function within the list
setmean = setmean,
getmean = getmean)
}
