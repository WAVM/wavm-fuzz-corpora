(module
  (type $ii-i (func (param i32 i32) (result i32)))
  (type $0 (func))
  (type $1 (func (param i32 i32 i32) (result i32)))
  (table $t1  2 2 funcref)
  (table $t2  3 3 funcref)
  (table $t3  4 funcref)
  (export "call-1" (func $6))
  (export "call-2" (func $7))
  (export "call-3" (func $8))
  (elem $2 (i32.const 0)
    $f $g)
  (elem $3 (table $t2) (i32.const 0)
    $h $i $j)
  (elem $4 (table $t3) (i32.const 0)
    $g $h)
  (elem $5 (table $t3) (i32.const 3)
    $z)
  
  (func $f (type $ii-i)
    (param $0 i32)
    (param $1 i32)
    (result i32)
    local.get $0
    local.get $1
    i32.add
    )
  
  (func $g (type $ii-i)
    (param $0 i32)
    (param $1 i32)
    (result i32)
    local.get $0
    local.get $1
    i32.sub
    )
  
  (func $h (type $ii-i)
    (param $0 i32)
    (param $1 i32)
    (result i32)
    local.get $0
    local.get $1
    i32.mul
    )
  
  (func $i (type $ii-i)
    (param $0 i32)
    (param $1 i32)
    (result i32)
    local.get $0
    local.get $1
    i32.div_u
    )
  
  (func $j (type $ii-i)
    (param $0 i32)
    (param $1 i32)
    (result i32)
    local.get $0
    local.get $1
    i32.rem_u
    )
  
  (func $z (type $0)
    )
  
  (func $6 (type $1)
    (param $0 i32)
    (param $1 i32)
    (param $2 i32)
    (result i32)
    local.get $0
    local.get $1
    local.get $2
    call_indirect $t1 (type $ii-i)
    )
  
  (func $7 (type $1)
    (param $0 i32)
    (param $1 i32)
    (param $2 i32)
    (result i32)
    local.get $0
    local.get $1
    local.get $2
    call_indirect $t2 (type $ii-i)
    )
  
  (func $8 (type $1)
    (param $0 i32)
    (param $1 i32)
    (param $2 i32)
    (result i32)
    local.get $0
    local.get $1
    local.get $2
    call_indirect $t3 (type $ii-i)
    ))