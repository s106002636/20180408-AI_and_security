--->matplotlib (如圖1-3)
import numpy as np
import matplotlib.pyplot as plt

a = [1,2,3]
b = [4,5,6]
plt.plot(a,b)

plt.plot(a,b,'*') """可換成點方式呈現"""

--->insow (如圖)
# coding: utf-8
# img_show.py

import matplotlib.pyplot as plt
from matplotlib.image import imread

img = imread('../Deep/dataset/lena.png') 
plt.imshow(img)

plt.show()

--->繪製sin (如圖)
# coding: utf-8
import numpy as np
import matplotlib.pyplot as plt

x = np.arange(0, 6, 0.1) 
y = np.sin(x)

plt.plot(x, y)
plt.show()

--->繪製sin有圖示及標體 (如圖)
# coding: utf-8
import numpy as np
import matplotlib.pyplot as plt

x = np.arange(0, 6, 0.1) 
y1 = np.sin(x)
y2 = np.cos(x)

plt.plot(x, y1, label="sin")
plt.plot(x, y2, linestyle = "--", label="cos")
plt.xlabel("x") 
plt.xlabel("y") 
plt.title('sin&cos')
plt.legend()
plt.show()
