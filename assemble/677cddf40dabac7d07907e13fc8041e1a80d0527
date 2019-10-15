(module
  (type $0 (func (result i32)))
  (type $1 (func))
  (type $2 (func (param i32) (result i32)))
  (memory $a  0)
  (memory $b  0)
  (export "a.load_at_zero" (func $3))
  (export "a.store_at_zero" (func $4))
  (export "a.load_at_page_size" (func $5))
  (export "a.store_at_page_size" (func $6))
  (export "a.grow" (func $7))
  (export "a.size" (func $8))
  (export "b.load_at_zero" (func $9))
  (export "b.store_at_zero" (func $10))
  (export "b.load_at_page_size" (func $11))
  (export "b.store_at_page_size" (func $12))
  (export "b.grow" (func $13))
  (export "b.size" (func $14))
  
  (func $3 (type $0)
    (result i32)
    i32.const 0
    i32.load
    )
  
  (func $4 (type $1)
    i32.const 0
    i32.const 2
    i32.store
    )
  
  (func $5 (type $0)
    (result i32)
    i32.const 65536
    i32.load
    )
  
  (func $6 (type $1)
    i32.const 65536
    i32.const 3
    i32.store
    )
  
  (func $7 (type $2)
    (param $sz i32)
    (result i32)
    local.get $sz
    memory.grow
    )
  
  (func $8 (type $0)
    (result i32)
    memory.size
    )
  
  (func $9 (type $0)
    (result i32)
    i32.const 0
    i32.load $b
    )
  
  (func $10 (type $1)
    i32.const 0
    i32.const 2
    i32.store $b
    )
  
  (func $11 (type $0)
    (result i32)
    i32.const 65536
    i32.load $b
    )
  
  (func $12 (type $1)
    i32.const 65536
    i32.const 3
    i32.store $b
    )
  
  (func $13 (type $2)
    (param $sz i32)
    (result i32)
    local.get $sz
    memory.grow $b
    )
  
  (func $14 (type $0)
    (result i32)
    memory.size $b
    ))