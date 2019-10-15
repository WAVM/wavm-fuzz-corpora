(module
  (type $0 (func (param i32 externref i32)))
  (type $1 (func (param i32) (result externref)))
  (table $t  10 externref)
  (export "fill" (func $2))
  (export "get" (func $3))
  
  (func $2 (type $0)
    (param $i i32)
    (param $r externref)
    (param $n i32)
    local.get $i
    local.get $r
    local.get $n
    table.fill $t
    )
  
  (func $3 (type $1)
    (param $i i32)
    (result externref)
    local.get $i
    table.get $t
    ))