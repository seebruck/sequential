Say you want to count by eights, from a given starting point (25) to a certain threshold (1000). Here are some ways to do that in R:

# For-Loop
```
for(i in seq(25,1000,8)) {
     print(i)
}

# or, more simply:
for(i in seq(25,1000,8)) print(i)
```

# While-Loop
```
x <- 25
while(x <= 1000) { 
    print(x <- x+8) 
}

# or, more simply:
x <- 25
while(x <= 1000) print(x <- x+8)
```

# Repeat-Loop
```
x <- 25
repeat {
  print(x)
  x <- x+8
  if (x >= 1000){
   break
 }
}
```

# Vector of Sequences
```
# or, the most parsimonious:
print(seq(25,1000,8))
print(seq(from = 25, to = 1000, by = 8))
```
