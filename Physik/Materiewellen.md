Photonen, welche lange zeit als Wellen anerkannt wurden, haben einen Impuls $p$ und somit auch einen Teilchencharakter. De Broglie hatte die Idee dies umgekehrt für Teilchen zu definieren. Somit lässt sich einem Teilchen mit einem Impuls $p$ eine Wellenlänge (Die De-Broglie Wellenlänge) zuordnen:
$$\lambda = \frac{h}{p}$$
Teilchen mit einer Wellenlänge (z.B. Elektronen oder Protonen) bezeichnet man als Materiewellen. Weiterführend verhalten sich Materiewellen auch wie Wellen, so lässt sich die Interferenz eines einzelnen Elektrons an einem Doppelspalt feststellen.

Wird ein Teilchen mit der Masse $m$ und Ladung $q$ anhand einer Beschleunigungsspannung $U$ beschleunigt, so gilt folgendes:
$$E_{kin} = qU$$
Da weiterführend gilt $E = \frac{p^2}{2m}$ ist der Impuls gegeben durch:
$$p = \sqrt{2qUm}$$
Somit hat dieses Teilchen eine Wellenlänge von:
$$\lambda = \frac{h}{\sqrt{2qUm}}$$
Die Wellenlänge von Materiewellen ist jedoch sehr gering, setzt man z.B. für $q$ die Elementarladung $e$ ein und für $m$ die masse eines Elektrons, ergibt sich folgendes:
$$\lambda(U) = \frac{6,6261 \cdot 10^{-34}Js}{\sqrt{2U \cdot 9,1097\cdot 10^{-31}kg \cdot 1,6022\cdot10^{-19}C}}$$


![[Pasted image 20231024204821.png]]
```python
import numpy as np
import scipy.constants as constants
import matplotlib.pyplot as plt


definition = 1000
maxvolt = 500

def nu(U):
	#multiply U by 1000 to convert Volt to kV
	p = np.sqrt(2 * constants.e * constants.m_e * U * 1000)
    return constants.h / p

U_in = np.linspace(1,maxvolt, num=definition)

Nu_out = nu(U_in)

plt.plot(U_in,Nu_out)
plt.show()
```

#quantenphysik 