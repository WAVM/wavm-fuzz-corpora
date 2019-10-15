(module
  (type $T (func (result i32)))
  (type $U (func (result i32)))
  (type $0 (func (param i32) (result i32)))
  (table $1  7 7 funcref)
  (export "callt" (func $3))
  (export "callu" (func $4))
  (elem $2 (i32.const 0)
    $t1 $t2 $t3 $u1 $u2 $t1 $t3)
  
  (func $t1 (type $T)
    (result i32)
    i32.const 1
    )
  
  (func $t2 (type $T)
    (result i32)
    i32.const 2
    )
  
  (func $t3 (type $T)
    (result i32)
    i32.const 3
    )
  
  (func $u1 (type $U)
    (result i32)
    i32.const 4
    )
  
  (func $u2 (type $U)
    (result i32)
    i32.const 5
    )
  
  (func $3 (type $0)
    (param $i i32)
    (result i32)
    local.get $i
    call_indirect $1 (type $T)
    )
  
  (func $4 (type $0)
    (param $i i32)
    (result i32)
    local.get $i
    call_indirect $1 (type $U)
    ))