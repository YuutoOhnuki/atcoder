# D
## 問題概要
道と障害物で構成されるgridが与えられる。
道に照明を設置したとき、照らされるマスの最大値を求める。

## 方法
 - 全探索
 - 縦方向と横方向について、それぞれ何マス照らすことができるかを管理
    - 片方から見ていき、最後に後ろから最大値を探索

# E
## 問題概要
以下の条件を満たす非負整数(a,b)の組み合わせ総数
 * a+b <= L 
 * a+b = a xor b

## 方法
 - bitDPかと思ったが、桁DPだった (制約からも桁DP)
 - 桁DPでは上から何文字目まで決めたか、L未満が確定しているかを管理
