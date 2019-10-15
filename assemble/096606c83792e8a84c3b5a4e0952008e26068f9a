(module
  (type $0 (func (param i32) (result f32)))
  (type $1 (func (param i32)))
  (memory $2  1)
  (export "32_good1" (func $4))
  (export "32_good2" (func $5))
  (export "32_good3" (func $6))
  (export "32_good4" (func $7))
  (export "32_good5" (func $8))
  (export "32_bad" (func $9))
  
  (func $4 (type $0)
    (param $i i32)
    (result f32)
    local.get $i
    f32.load
    )
  
  (func $5 (type $0)
    (param $i i32)
    (result f32)
    local.get $i
    f32.load align=1
    )
  
  (func $6 (type $0)
    (param $i i32)
    (result f32)
    local.get $i
    f32.load offset=1 align=1
    )
  
  (func $7 (type $0)
    (param $i i32)
    (result f32)
    local.get $i
    f32.load offset=2 align=2
    )
  
  (func $8 (type $0)
    (param $i i32)
    (result f32)
    local.get $i
    f32.load offset=8
    )
  
  (func $9 (type $1)
    (param $i i32)
    local.get $i
    f32.load offset=4294967295
    drop
    )
  
  (data $3 (i32.const 0)
    "\00\00\00\00\00\00\a0\7f\01\00\d0\7f"))