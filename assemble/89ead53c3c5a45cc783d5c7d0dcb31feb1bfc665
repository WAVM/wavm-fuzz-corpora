(module
  (type $0 (func (result i32)))
  (import "M" "mem1" (memory $mem1 1 5))
  (import "M" "mem2" (memory $mem2 0))
  (memory $mem3  3)
  (memory $mem4  4 5)
  (export "size1" (func $1))
  (export "size2" (func $2))
  (export "size3" (func $3))
  (export "size4" (func $4))
  
  (func $1 (type $0)
    (result i32)
    memory.size
    )
  
  (func $2 (type $0)
    (result i32)
    memory.size $mem2
    )
  
  (func $3 (type $0)
    (result i32)
    memory.size $mem3
    )
  
  (func $4 (type $0)
    (result i32)
    memory.size $mem4
    ))