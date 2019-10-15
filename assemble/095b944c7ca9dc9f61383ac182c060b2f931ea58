(module
  (type $0 (func))
  (type $1 (func (param externref)))
  (type $2 (func (param i32) (result externref)))
  (type $3 (func (param i32) (result funcref)))
  (type $4 (func (param i32) (result i32)))
  (table $t2  2 externref)
  (table $t3  3 funcref)
  (export "init" (func $6))
  (export "get-externref" (func $7))
  (export "get-funcref" (func $f3))
  (export "is_null-funcref" (func $8))
  (elem $5 (table $t3) (i32.const 1)
    $dummy)
  
  (func $dummy (type $0)
    )
  
  (func $6 (type $1)
    (param $r externref)
    i32.const 1
    local.get $r
    table.set $t2
    i32.const 2
    i32.const 1
    table.get $t3
    table.set $t3
    )
  
  (func $7 (type $2)
    (param $i i32)
    (result externref)
    local.get $i
    table.get $t2
    )
  
  (func $f3 (type $3)
    (param $i i32)
    (result funcref)
    local.get $i
    table.get $t3
    )
  
  (func $8 (type $4)
    (param $i i32)
    (result i32)
    local.get $i
    call $f3
    ref.is_null
    ))