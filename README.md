# Array
Common Lisp eDSL for operations on array-like containers

<br>

## API

<br>

## Examples

#### Get element index

List:
```common-lisp
(let ((lst-1 '(1 5 9 7))
      (lst-2 '((1 2) (3 4) (5 6))))

  (index 9 lst-1))                                  ; => 2
  (index '(3 4) lst-2 :test #'equalp))              ; => 1
```

Vector:
```common-lisp
(index 0 #(1 2 3 0 4 5))                             ; => 3
(index inst-2 #(inst-1 inst-2 inst-3) :test #'eq)    ; => 1
```

Array:
```common-lisp
(index 17 :axis 1 #2a((26 8) (17 3) (12 5))          ; => '(1 0)
```

<br>

#### Get slice

List:
```common-lisp
(slice  0)
(slice)
```

Vector:
```common-lisp
(slice)
```

Array:
```common-lisp
(slice)
```



