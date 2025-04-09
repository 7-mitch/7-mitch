# 7-mitch
import numpy as np
import matplotlib.pyplot as plt

# データの生成: 0 から 2π までの 100 点
x = np.linspace(0, 2 * np.pi, 100)
y_sin = np.sin(x)
y_cos = np.cos(x)

# プロットの作成
plt.figure(figsize=(8, 4))

# サイン波をプロット（青色、実線）
plt.plot(x, y_sin, label='sin(x)', color='blue', linestyle='-')

# コサイン波をプロット（赤色、破線）
plt.plot(x, y_cos, label='cos(x)', color='red', linestyle='--')

# グラフタイトル、軸ラベルの設定
plt.title("Sine and Cosine Waves")
plt.xlabel("x")
plt.ylabel("y")

# 凡例の表示
plt.legend()

# グリッドの表示
plt.grid(True)

# グラフの表示
plt.show()
