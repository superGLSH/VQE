## Постановка

Задача укладки рюкзака

## QUBO-модель

Задача QUBO ставится следующим образом:

$$QUBO = A\left(W - \sum_1^nw_ix_i- \sum_1^{\log_2(w_{max} +1)}2^{i-1}y_i\right)^2-\sum_1^nv_ix_i$$
Раскрывая скобки и игнорируя константы, получим:
$$QUBO=2A (\sum _ {i\ne{j}} w_iw_jx_ix_j +
\sum _ {i\ne{j}} 2^{i+j-2}y_iy_j +
\sum _ {i, j} 2^{i-1}w_jx_jy_i - 
W_{max}\sum_1^nw_ix_i - W_{max}\sum_1^n2^{i-1}y_i)\
-\sum_1^nv_ix_i$$