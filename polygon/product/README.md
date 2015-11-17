# Matrixの掛け算
Matrixには、足し算、引き算、掛け算などがあります。
掛け算について学びましょう。


## 掛け算する事で、回転後の位置が決まる


$$ \left(
\begin{array}{ccc}
x_{next} \\
y_{next} \\
z_{next} \\
1 \\
\end{array}
\right)
=
\left(\begin{array}{ccc}
\\
回転行列\\
\\
\end{array}
\right)
\left(
\begin{array}{ccc}
x \\
y \\
z \\
1 \\
\end{array}
\right)
$$

こんな感じて、掛け算する事で、回転後の位置を求める事ができまする
$$\left(x, y, z\right)$$の点に回転行列をかける事で、回転後の$$ \left(x_{next},y_{next},z_{next}\right)$$の位置が求まります。

<br>

Matrixの掛け算を実装してみましょう。


