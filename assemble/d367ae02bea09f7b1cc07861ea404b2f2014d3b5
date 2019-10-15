(module
  (type $0 (func (param f32) (result f32)))
  (type $1 (func (param f64) (result f64)))
  (export "f32.no_fold_lt_if_to_abs" (func $2))
  (export "f32.no_fold_le_if_to_abs" (func $3))
  (export "f32.no_fold_gt_if_to_abs" (func $4))
  (export "f32.no_fold_ge_if_to_abs" (func $5))
  (export "f64.no_fold_lt_if_to_abs" (func $6))
  (export "f64.no_fold_le_if_to_abs" (func $7))
  (export "f64.no_fold_gt_if_to_abs" (func $8))
  (export "f64.no_fold_ge_if_to_abs" (func $9))
  
  (func $2 (type $0)
    (param $x f32)
    (result f32)
    local.get $x
    f32.const 0x0.000000p-127
    f32.lt
    if $if (result f32)
      local.get $x
      f32.neg
    else
      local.get $x
    end ;; $if
    )
  
  (func $3 (type $0)
    (param $x f32)
    (result f32)
    local.get $x
    f32.const -0x0.000000p-127
    f32.le
    if $if (result f32)
      local.get $x
      f32.neg
    else
      local.get $x
    end ;; $if
    )
  
  (func $4 (type $0)
    (param $x f32)
    (result f32)
    local.get $x
    f32.const -0x0.000000p-127
    f32.gt
    if $if (result f32)
      local.get $x
    else
      local.get $x
      f32.neg
    end ;; $if
    )
  
  (func $5 (type $0)
    (param $x f32)
    (result f32)
    local.get $x
    f32.const 0x0.000000p-127
    f32.ge
    if $if (result f32)
      local.get $x
    else
      local.get $x
      f32.neg
    end ;; $if
    )
  
  (func $6 (type $1)
    (param $x f64)
    (result f64)
    local.get $x
    f64.const 0x0.0000000000000p-1023
    f64.lt
    if $if (result f64)
      local.get $x
      f64.neg
    else
      local.get $x
    end ;; $if
    )
  
  (func $7 (type $1)
    (param $x f64)
    (result f64)
    local.get $x
    f64.const -0x0.0000000000000p-1023
    f64.le
    if $if (result f64)
      local.get $x
      f64.neg
    else
      local.get $x
    end ;; $if
    )
  
  (func $8 (type $1)
    (param $x f64)
    (result f64)
    local.get $x
    f64.const -0x0.0000000000000p-1023
    f64.gt
    if $if (result f64)
      local.get $x
    else
      local.get $x
      f64.neg
    end ;; $if
    )
  
  (func $9 (type $1)
    (param $x f64)
    (result f64)
    local.get $x
    f64.const 0x0.0000000000000p-1023
    f64.ge
    if $if (result f64)
      local.get $x
    else
      local.get $x
      f64.neg
    end ;; $if
    ))