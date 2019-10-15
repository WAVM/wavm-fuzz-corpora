(module
  (type $0 (func (result i32)))
  (type $1 (func (param i32 i32)))
  (type $2 (func (param i32) (result i32)))
  (memory $3  1)
  (export "store" (func $4))
  (export "load" (func $5))
  (export "memory.grow" (func $6))
  
  (func $addr_limit (type $0)
    (result i32)
    memory.size
    i32.const 65536
    i32.mul
    )
  
  (func $4 (type $1)
    (param $i i32)
    (param $v i32)
    call $addr_limit
    local.get $i
    i32.add
    local.get $v
    i32.store
    )
  
  (func $5 (type $2)
    (param $i i32)
    (result i32)
    call $addr_limit
    local.get $i
    i32.add
    i32.load
    )
  
  (func $6 (type $2)
    (param $0 i32)
    (result i32)
    local.get $0
    memory.grow
    ))