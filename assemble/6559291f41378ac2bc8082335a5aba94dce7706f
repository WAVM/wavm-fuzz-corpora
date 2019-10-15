(module
  (type $0 (func (param funcref) (result i32)))
  (type $1 (func (param externref) (result i32)))
  (type $2 (func))
  (type $3 (func (param externref)))
  (type $4 (func (param i32) (result i32)))
  (table $t1  2 funcref)
  (table $t2  2 externref)
  (export "funcref" (func $f1))
  (export "externref" (func $f2))
  (export "init" (func $6))
  (export "deinit" (func $7))
  (export "funcref-elem" (func $8))
  (export "externref-elem" (func $9))
  (elem $5 (i32.const 1)
    $dummy)
  
  (func $f1 (type $0)
    (param $x funcref)
    (result i32)
    local.get $x
    ref.is_null
    )
  
  (func $f2 (type $1)
    (param $x externref)
    (result i32)
    local.get $x
    ref.is_null
    )
  
  (func $dummy (type $2)
    )
  
  (func $6 (type $3)
    (param $r externref)
    i32.const 1
    local.get $r
    table.set $t2
    )
  
  (func $7 (type $2)
    i32.const 1
    ref.null func
    table.set $t1
    i32.const 1
    ref.null extern
    table.set $t2
    )
  
  (func $8 (type $4)
    (param $x i32)
    (result i32)
    local.get $x
    table.get $t1
    call $f1
    )
  
  (func $9 (type $4)
    (param $x i32)
    (result i32)
    local.get $x
    table.get $t2
    call $f2
    ))