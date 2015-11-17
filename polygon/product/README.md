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

### 掛け算のルール

$$ \left(
\begin{array}{ccc}
x_{next} \\
y_{next} \\
z_{next} \\
1 \\
\end{array}
\right)
=
\left(
  \begin{array}{ccc}
    a_{11} & a_{12} & a_{13} & a_{14}\\
    a_{21} & a_{22} & a_{23} & a_{24}\\
    a_{31} & a_{32} & a_{33} & a_{34}\\
    a_{41} & a_{42} & a_{43} & a_{44}\\
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
=
\left(
\begin{array}{ccc}
a_{11} \times x + a_{12} \times y + a_{13} \times z + a_{14} \times 1\\
a_{21} \times x + a_{22} \times y + a_{23} \times z + a_{24} \times 1\\
a_{31} \times x + a_{32} \times y + a_{33} \times z + a_{34} \times 1\\
a_{41} \times x + a_{42} \times y + a_{43} \times z + a_{44} \times 1\\
\end{array}
\right)
$$


