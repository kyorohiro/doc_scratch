# Y軸で回転する


見た目が変わらないのはここまで。ポリゴンを回転させて見ましょう。


$$ 
\left(\begin{array}{ccc}
\cos\theta & 0 & \sin\theta & 0 \\
0 & 1 & 0 & 0 \\
-\sin\theta & 0 & \cos\theta & 0 \\
0 & 0 & 0 & 1 \\
\end{array}
\right)
$$

<br>
<br>


## 回転した後の値
$$ 
\left(
  \begin{array}{ccc}
    a_{11} & a_{12} & a_{13} & a_{14}\\
    a_{21} & a_{22} & a_{23} & a_{24}\\
    a_{31} & a_{32} & a_{33} & a_{34}\\
    a_{41} & a_{42} & a_{43} & a_{44}\\
  \end{array}
\right)
\left(\begin{array}{ccc}
\cos\theta & 0 & \sin\theta & 0 \\
0 & 1 & 0 & 0 \\
-\sin\theta & 0 & \cos\theta & 0 \\
0 & 0 & 0 & 1 \\
\end{array}
\right)
=
\left(
  \begin{array}{ccc}
    M_{11} & a_{12} & M_{13} & a_{14}\\
    M_{21} & a_{22} & M_{23} & a_{24}\\
    M_{31} & a_{32} & M_{33} & a_{34}\\
    M_{41} & a_{42} & M_{43} & a_{44}\\
  \end{array}
\right)
$$

$$\\
M_{11} = a_{11} \times \cos\theta + a_{13} \times \sin\theta \\
M_{21} = a_{21} \times \cos\theta + a_{23} \times \sin\theta \\
M_{31} = a_{31} \times \cos\theta + a_{33} \times \sin\theta \\
M_{41} = a_{41} \times \cos\theta + a_{43} \times \sin\theta \\
$$

$$\\
M_{13} = a_{11} \times -\sin\theta + a_{23} \times \cos\theta \\
M_{23} = a_{21} \times -\sin\theta + a_{23} \times \cos\theta \\
M_{33} = a_{31} \times -\sin\theta + a_{33} \times \cos\theta \\
M_{43} = a_{41} \times -\sin\theta + a_{43} \times \cos\theta \\
$$

<br>
<br>
## Scratchで実装してみよう

### (1) スクリプト画面を表示
![](k001.png)
##### (1-1) 左下のSprite1をクリック
##### (1-2) スクリプトタブをクリック

<br>
<br>
<br>

### (2) 回転スクリプトを追加
![](ks01.png)

<br>
<br>
### (2-注) 

![](ks01_opt1.png)
##### ブロックを作成するときは、「画面を再描画せずに実行する」チェックを入れること

<br>
<br>
### (3) 確認する
![](ks02.png)
##### (3-1) 旗がクリックされた時の、コードを変更する

<br>
<br>
https://scratch.mit.edu/projects/88153625/

![](kc01.png)

##### (3-2) 右上の旗をクリック
##### (3-3) 三角形が回転すること

<br>
<br>

### (4) Good!
![](../good.png)


