(module
  (type $0 (func))
  (type $1 (func (result i32)))
  (memory $2  1 1)
  (export "inc" (func $inc))
  (export "get" (func $get))
  (start $main)
  
  (func $inc (type $0)
    i32.const 0
    i32.const 0
    i32.load8_u
    i32.const 1
    i32.add
    i32.store8
    )
  
  (func $get (type $1)
    (result i32)
    i32.const 0
    i32.load8_u
    return
    )
  
  (func $main (type $0)
    call $inc
    call $inc
    call $inc
    )
  
  (data $3 (i32.const 0)
    "A"))