(module
  (type $0 (func))
  (memory $1  1)
  (export "as-block-value" (func $2))
  (export "as-loop-value" (func $3))
  (export "as-br-value" (func $4))
  (export "as-br_if-value" (func $5))
  (export "as-br_if-value-cond" (func $6))
  (export "as-br_table-value" (func $7))
  (export "as-return-value" (func $8))
  (export "as-if-then" (func $9))
  (export "as-if-else" (func $10))
  
  (func $2 (type $0)
    block $block
      i32.const 0
      i32.const 1
      i32.store
    end ;; $block
    )
  
  (func $3 (type $0)
    loop $loop
      i32.const 0
      i32.const 1
      i32.store
    end ;; $loop
    )
  
  (func $4 (type $0)
    block $block
      i32.const 0
      i32.const 1
      i32.store
      br $block
    end ;; $block
    )
  
  (func $5 (type $0)
    block $block
      i32.const 0
      i32.const 1
      i32.store
      i32.const 1
      br_if $block
    end ;; $block
    )
  
  (func $6 (type $0)
    block $block
      i32.const 6
      i32.const 0
      i32.const 1
      i32.store
      br_if $block
    end ;; $block
    )
  
  (func $7 (type $0)
    block $block
      i32.const 0
      i32.const 1
      i32.store
      i32.const 1
      br_table
        $block ;; default
    end ;; $block
    )
  
  (func $8 (type $0)
    i32.const 0
    i32.const 1
    i32.store
    return
    )
  
  (func $9 (type $0)
    i32.const 1
    if $if
      i32.const 0
      i32.const 1
      i32.store
    end ;; $if
    )
  
  (func $10 (type $0)
    i32.const 0
    if $if
    else
      i32.const 0
      i32.const 1
      i32.store
    end ;; $if
    ))