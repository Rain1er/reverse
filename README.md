## JCC 指令

| **指令** | **描述**                        | **标志位**       |
| -------- | ------------------------------- | ---------------- |
| je、jz | 结果为零则跳转 (相等时跳转)     | ZF=1             |
| jne、jnz | 结果不为零则跳转 (不相等时跳转) | ZF=0             |
| js       | 结果为负则跳转                  | SF=1             |
| jns      | 结果为非负则跳转                | SF=0             |
| jp、jpe | 结果中1的个数为偶数则跳转       | PF=1             |
| jnp、jpo | 结果中1的个数为奇数则跳转       | PF=0             |
| jo       | 结果溢出则跳转                  | OF=1             |
| jno      | 结果没有溢出则跳转              | OF=0             |
| jnb、jae | 大于等于则跳转 (无符号数)       | CF=0             |
| jbe、jna | 小于等于则跳转 (无符号数)       | CF=1 or ZF=1     |
| jnbe、ja | 大于则跳转 (无符号数)           | CF=0 and ZF=0    |
| jb、jnae | 小于则跳转 (无符号数)           | CF=1             |
| jnl、jge | 大于等于则跳转 (有符号数)       | SF=OF            |
| jle、jng | 小于等于则跳转 (有符号数)       | ZF=1 or SF \\= OF |
| jnle、jg | 大于则跳转 (有符号数)           | ZF=0 and SF=OF   |
| jl、jnge | 小于则跳转 (有符号数)           | SF \\= OF        |
