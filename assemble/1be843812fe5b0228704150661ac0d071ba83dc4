(module
  (type $0 (func (result i32)))
  (type $1 (func (param i32) (result i32)))
  (import "M" "mem1" (memory $mem1 1 6))
  (import "M" "mem2" (memory $mem2 0))
  (memory $mem3  3)
  (memory $mem4  4 5)
  (export "size1" (func $2))
  (export "size2" (func $3))
  (export "size3" (func $4))
  (export "size4" (func $5))
  (export "grow1" (func $6))
  (export "grow2" (func $7))
  (export "grow3" (func $8))
  (export "grow4" (func $9))
  
  (func $2 (type $0)
    (result i32)
    memory.size
    )
  
  (func $3 (type $0)
    (result i32)
    memory.size $mem2
    )
  
  (func $4 (type $0)
    (result i32)
    memory.size $mem3
    )
  
  (func $5 (type $0)
    (result i32)
    memory.size $mem4
    )
  
  (func $6 (type $1)
    (param $0 i32)
    (result i32)
    local.get $0
    memory.grow
    )
  
  (func $7 (type $1)
    (param $0 i32)
    (result i32)
    local.get $0
    memory.grow $mem2
    )
  
  (func $8 (type $1)
    (param $0 i32)
    (result i32)
    local.get $0
    memory.grow $mem3
    )
  
  (func $9 (type $1)
    (param $0 i32)
    (result i32)
    local.get $0
    memory.grow $mem4
    ))