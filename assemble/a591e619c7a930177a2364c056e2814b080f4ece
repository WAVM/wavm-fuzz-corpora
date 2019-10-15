(module
  (type $0 (func (param v128 v128 v128) (result v128)))
  (type $1 (func (param v128 v128) (result v128)))
  (export "add-sub" (func $2))
  (export "mul-add" (func $3))
  (export "mul-sub" (func $4))
  (export "sub-add" (func $5))
  (export "add-neg" (func $6))
  (export "mul-neg" (func $7))
  (export "sub-neg" (func $8))
  
  (func $2 (type $0)
    (param $0 v128)
    (param $1 v128)
    (param $2 v128)
    (result v128)
    local.get $0
    local.get $1
    i16x8.sub
    local.get $2
    i16x8.add
    )
  
  (func $3 (type $0)
    (param $0 v128)
    (param $1 v128)
    (param $2 v128)
    (result v128)
    local.get $0
    local.get $1
    i16x8.add
    local.get $2
    i16x8.mul
    )
  
  (func $4 (type $0)
    (param $0 v128)
    (param $1 v128)
    (param $2 v128)
    (result v128)
    local.get $0
    local.get $1
    i16x8.sub
    local.get $2
    i16x8.mul
    )
  
  (func $5 (type $0)
    (param $0 v128)
    (param $1 v128)
    (param $2 v128)
    (result v128)
    local.get $0
    local.get $1
    i16x8.add
    local.get $2
    i16x8.sub
    )
  
  (func $6 (type $1)
    (param $0 v128)
    (param $1 v128)
    (result v128)
    local.get $0
    i16x8.neg
    local.get $1
    i16x8.add
    )
  
  (func $7 (type $1)
    (param $0 v128)
    (param $1 v128)
    (result v128)
    local.get $0
    i16x8.neg
    local.get $1
    i16x8.mul
    )
  
  (func $8 (type $1)
    (param $0 v128)
    (param $1 v128)
    (result v128)
    local.get $0
    i16x8.neg
    local.get $1
    i16x8.sub
    ))