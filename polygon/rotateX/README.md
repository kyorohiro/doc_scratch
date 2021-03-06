# X軸(じく)で回転(かいてん)する

![](about.png)

<br>
<br>


## 回転(かいてん)した後(あと)の値(あたい)
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
1 & 0 & 0 & 0 \\
0 & \cos\theta & -\sin\theta & 0\\
0 & \sin\theta & \cos\theta & 0\\
0 & 0 & 0 & 1\\
\end{array}
\right)
=
\left(
  \begin{array}{ccc}
    a_{11} & M_{12} & M_{13} & a_{14}\\
    a_{21} & M_{22} & M_{23} & a_{24}\\
    a_{31} & M_{32} & M_{33} & a_{34}\\
    a_{41} & M_{42} & M_{43} & a_{44}\\
  \end{array}
\right)
$$

$$\\
M_{12} = a_{12} \times \cos\theta + a_{13} \times \sin\theta \\
M_{22} = a_{22} \times \cos\theta + a_{23} \times \sin\theta \\
M_{32} = a_{32} \times \cos\theta + a_{33} \times \sin\theta \\
M_{42} = a_{42} \times \cos\theta + a_{43} \times \sin\theta \\
$$

$$\\
M_{13} = a_{12} \times -\sin\theta + a_{23} \times \cos\theta \\
M_{23} = a_{22} \times -\sin\theta + a_{23} \times \cos\theta \\
M_{33} = a_{32} \times -\sin\theta + a_{33} \times \cos\theta \\
M_{43} = a_{42} \times -\sin\theta + a_{43} \times \cos\theta \\
$$

<br>
<br>
## Scratchで実装(じっそう)してみよう

### (1) スクリプト画面(がめん)を表示(ひょうじ)
![](h001.png)
##### (1-1) 左下(ひだりした)のSprite1をクリック
##### (1-2) スクリプトタブをクリック

<br>
<br>
<br>

### (2) 回転(かいてん)スクリプトを追加(ついか)
![](hs01.png)

<br>
<br>
### (2-注) 

![](hs01_opt1.png)
##### ブロックを作成(さくせい)するときは、「画面を再描画せずに実行する」チェックを入(い)れること

<br>
<br>
### (3) 確認(かくにん)する
![](hs02.png)
##### (3-1) 旗(はた)がクリックされた時(とき)の、コードを変更(へんこう)する

<br>
<br>
https://scratch.mit.edu/projects/88146325/

![](hc01.png)

##### (3-2) 右上(みぎうえ)の旗(はた)をクリック
##### (3-3) 三角形(さんかっけい)が回転(かいてん)すること

<br>
<br>

### (4) Good!
![](../good.png)

よくできました。次(つぎ)のステップに進(すす)みましょう。


