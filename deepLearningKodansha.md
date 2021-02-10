# 順伝播型ネットワーク

## 概要

順伝播型ネットワーク = 多層パーセプトロン

一つのパーセプトロンの構成

![IMG_321124CB943D-1](/Users/okpn/Downloads/IMG_321124CB943D-1.jpeg)
$$
z = f(u) = f(w_1x_1+w_2x_2+w_3x_3+w_4x_4 + b)
$$
重さwは，かく入力がどれくらいの重要度で入力されるかの係数



一つのパーセプトロンの層が多層に重なっているのが多層パーセプトロン

![IMG_138D040B151A-1](/Users/okpn/Downloads/IMG_138D040B151A-1.jpeg)

全結合の場合，全てのuに対して，前の層からの入力が重さをかけて入力される。前の層のノードの数をn個とし，uがm個あるとして一般化する。
$$
u_m = \sum_{i = 1}^{n} w_{mi}x_i+b_i\\
z_m = f(u_m)
$$
となる。これを行列で表すと，
$$
\begin{bmatrix}
	u_1\\
	\vdots\\
	u_n
\end{bmatrix}
= 
\begin{bmatrix}
	w_{11}&\cdots&w_{1n} \\
	\vdots&\ddots&\vdots \\
	w_{m1}&\cdots&w_{mn}
\end{bmatrix}
.
\begin{bmatrix}
	b_1\\
	\vdots\\
	b_n
\end{bmatrix}
$$
ここで以下のように配列を定義すると，
$$
u = 
\begin{bmatrix}
	u_1\\
	\vdots\\
	u_n
\end{bmatrix},
x = 
\begin{bmatrix}
	x_1\\
	\vdots\\
	x_n
\end{bmatrix},

b =
\begin{bmatrix}
	b_1\\
	\vdots\\
	b_n
\end{bmatrix}

z = 
\begin{bmatrix}
 z_1\\
 \vdots\\
 z_n
\end{bmatrix}\\

W = 
\begin{bmatrix}
	w_{11}&\cdots&w_{1n} \\
	\vdots&\ddots&\vdots \\
	w_{m1}&\cdots&w_{mn}
\end{bmatrix},
f(u)=
\begin{bmatrix}
	f(u_1)\\
	\vdots\\
	f(u_n)
\end{bmatrix} \\

$$



$$

$$
