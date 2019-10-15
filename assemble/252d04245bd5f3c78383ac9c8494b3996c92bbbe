(module
  (type $0 (func (param f64 f32) (result f32)))
  (type $1 (func (param f32 f64) (result f32)))
  (export "no_demote_mixed_add" (func $2))
  (export "no_demote_mixed_add_commuted" (func $3))
  
  (func $2 (type $0)
    (param $x f64)
    (param $y f32)
    (result f32)
    local.get $x
    local.get $y
    f64.promote_f32
    f64.add
    f32.demote_f64
    )
  
  (func $3 (type $1)
    (param $y f32)
    (param $x f64)
    (result f32)
    local.get $y
    f64.promote_f32
    local.get $x
    f64.add
    f32.demote_f64
    ))