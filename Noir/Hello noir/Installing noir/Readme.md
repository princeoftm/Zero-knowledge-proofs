we will need to install the Noir toolchain. To do so, run the following command.


```
curl -L https://raw.githubusercontent.com/noir-lang/noirup/main/install | bash

```


Recall that zkSNARKs generally prove the following statement: "I know a secret 
𝑤
 such 
𝐹
(
𝑥
,
𝑤
)
=
𝑦
". In Noir, we can easily define the logic of 
𝐹
, and interpretations (i.e., data types) for 
𝑥
, 
𝑤
, and 
𝑦
.