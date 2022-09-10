# taller3.graficadispersion
import numpy as np
import matplotlib.pyplot as plt
x = 10*np.random.rand(200, 1)
y = (0.2 + 0.8*x) * np.sin(2*np.pi*x) + \
     np.random.randn(200, 1)
     
x1= 10*np.random.rand(200, 1)
y2= (0.2 + 0.9*x) * np.cos(2*np.pi*x) + \
     np.random.randn(200, 1)
     
     
plt.scatter(x,y)
plt.show()
fig, ax = plt.subplots(5, 2, sharey = True)
ax[0, 0].scatter(x,y,color = 'orange')
ax[1, 0].scatter(x1,y2,color = 'violet')
ax[2, 0].scatter(x,y,color = 'red')
ax[3, 0].scatter(x1,y2,color = 'green')
ax[4, 0].scatter(x,y,color = 'orange')
ax[1, 1].scatter(x1,y2,color = 'blue')
ax[0, 1].scatter(x,y,color = 'red')
ax[2, 1].scatter(x1,y2,color = 'green')
ax[3, 1].scatter(x,y,color = 'orange')
ax[4, 1].scatter(x,y,color = 'violet')
