---
published: true
title: "Clojure By Example"
layout: post
tags: [clojure]
---

### Hello World
The entrie line of the code (....) is called a form in Clojure
```
(println "Hello World")
```

### Bindings
We call the mapping between names and values binding in Clojure

- Symbol

- Let
To bind values to names, use let
```
(let [a "aaaaa"] (println a))
```

- Scope

- Def

### Functions
- Defn

- Fn (Anonymous Funtion)
#() is the shortcut for fn

- Closure 

### Namespaces
- Create-ns
- In-ns
- Require
- Refer
- Use
- Import
- Ns

### Control Flow
- If
- If-Let
- When
- When-Let
- Case
- Cond
- Condp

### Boolean

### String
- Literal
- Str
- Format

### Intergers
- Addition / Subtraction / Multiplication / Division / Modulo 
- Max / Min / Power / Bigint

### Lists
- Literal 
```
`(1 2 3)
=> (1 2 3)
```

- Conj
```
(conj `(1 2 3) 4)
=> (4 1 2 3)
```

- Nth 
```
(nth '(1 2 3) 1)
=> 2
```

- Count
```
(count `(1 2 3))
=> 3
```

### Vector
- Literal / Conj / Nth / First / Last
```
[1 2 3]
```

- .indexOf
```
(.indexOf [1 2 3] 2)
=> 1
```

### Sets
- Literal / Conj (not duplicated values)
```
(conj (conj #{1 2 3} 4) 4)
=> #{ 1 4 2 3}
```

- Disj (remove item)
```
(disj #{1 2 3} 3)
=> #{1 2}
```

- Sort
```
(sort (conj #{1 2 3} 4))
=> (1 2 3 4)
```

- Contains?
```
(contains? #{1 2 3} 1)
=> true
```
- Subset?
```
(clojure.set/subset? #{1 2} #{1 2 3 4})
=> true
```
- Superset?
```
(clojure.set/superset? #{1 2 3} #{1 2})
=> true
```

### Map
- Literal
- Get
- Assoc
- Merge
- Keys
- Vals

### Sequences

