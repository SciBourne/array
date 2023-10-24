# Array
Common Lisp eDSL for operations on array-like containers

<br>

## Table of Contents

* [API Reference](#api-reference)
  * [Make](#make)
    * [List](#list)
    * [Array](#array)
    * [Vector](#vector)
    * [Stack](#stack)
    * [Queue](#queue)
    * [Double ended queue](#double-ended-queue)    
  * [Index](#index)
    * [List](#list-1)
    * [Array](#array-1)
    * [Vector](#vector-1)
  * [Slice](#slice)
    * [List](#list-2)
    * [Array](#array-2)
    * [Vector](#vector-2)

<br>

## API Reference

<br>

### Make

#### List

#### Array

#### Vector

#### Stack

#### Queue

#### Double ended queue

### Index

#### List

```common-lisp
(let ((lst-a '(1 5 9 7))
      (lst-b '((1 2)
               (3 4)
               (5 6))))

  (index 9 lst-a)                                  ; => 2
  (index '(3 4) lst-b :test #'equalp))             ; => 1
```

#### Array

```common-lisp
(let ((arr #2a((26 8)
               (17 3)
               (12 5))))

  (index 17 :axis 1 arr)                           ; => (1 0)
```

#### Vector

```common-lisp
(let ((vec-a #(1 2 3 0 4 5))
      (vec-b #(instance-1
               instance-2
               instance-3)))

  (index 0 vec-a)                                  ; => 3
  (index inst-b vec-b :test #'eq))                 ; => 1
```

### Slice

#### List

```common-lisp
(let ((lst-a '(1 2 3 4 5))
      (lst-b '((1 2)
               (3 4)
               (5 6))))

  (slice arr-a 0)                                  ; => 1
  (slice arr-a 3)                                  ; => 4
  (slice arr-a -1)                                 ; => 5
  (slice arr-a -3)                                 ; => 3

  (slice arr-a 3.5.-2 
```

#### Array

```common-lisp
(slice)
```

#### Vector

```common-lisp
(slice)
```





