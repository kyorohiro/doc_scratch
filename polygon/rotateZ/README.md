# Z軸で回転する

見た目が変わらないのはここまで。ポリゴンを回転させて見ましょう。


$$ 
\left(\begin{array}{ccc}
\cos\theta & -\sin\theta & 0 & 0\\
\sin\theta & \cos\theta & 0 & 0\\
0 & 0 & 1 & 0\\
0 & 0 & 0 & 1\\
\\
\end{array}
\right)
$$


## 行列同士の掛け算



## 回転した後の値



## Scratchで実装してみよう


<br>
<br>
<br>


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