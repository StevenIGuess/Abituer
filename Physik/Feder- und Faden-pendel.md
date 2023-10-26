#### Federpendel
Bei dem Federpendel, pendelt ein Masse -Stück, wegen einer Feder. Hierbei gilt das Hookesche Gesetz:
$$ F(x) = -Dx$$
Wobei $D$ ein Feder-spezifische Konstante (Einheit $\frac{N}{m}$) ist. Somit ist das [[Lineares Kraftgesetz|lineare Kraftgesetz]] erfüllt. Diese Schwingung lässt sich somit folgendermaßen beschreiben:
$$ x(t) = A\sin(\sqrt \frac{D}{m} \cdot t) + B \cos (\sqrt \frac{D}{m} \cdot t)$$
Wobei $A$ und $B$ durch Randbedingungen gegeben werden. Es gilt somit auch $\omega = \sqrt{\frac{D}{m}}$, wobei $\omega$ die Kreisfrequenz ist. Bewegt sich das Massenstück zwischen zwei Federn so gilt das Kompositionsprinzip: 
$$ F_{tot} (x) = F_1 + F_2 = (-D_1\cdot D_2) x$$
Somit verhält sich dieses System gleich.

![[Pasted image 20231026160103.png]]


### Fadenpendel
Bei einem Fadenpendel ist ein Masse-Stück an einem Faden befestigt. Diese Masse-Stück wird nun ausgelenkt und schwingt hin und her. Dies lässt sich Mathematisch folgendermaßen beschreiben:  

##### Newtonian
Auf das Masse-Stück wirkt die Erdanziehungskraft $m \cdot g$, jedoch trägt nur der tangentiale Teil dieser Kraft zur Bewegung bei:
![[Pasted image 20231026160559.png]]

Dieser Teil wird durch $mg \sin (\theta)$ gegeben. Aus dem ersten N. Gesetzt folgt nun:
$$ m \frac{d^2s}{dt} = -mg\sin(\theta)$$
Hierbei ist $s$ die Zurückgelegte Strecke. Es gilt weiterführend $\theta = \frac{s}{l}$, somit gilt:
$$ m \frac{d^2s}{dt} = -mg\sin(\frac{s}{l})$$
$$\Longleftrightarrow  \frac{d^2s}{dt} = -\frac{g}{l}\sin(s)$$
Ersetzt man nun $k= \frac{g}{k}$, und nimmt an das für kleine Auslenkungen $\sin(s) = s$ gilt, erhält man die Gleichung des [[Lineares Kraftgesetz|linearen Kraftgesetz]], somit gilt weiterführend:
$$ s(t) = A\sin(\sqrt \frac{g}{l} \cdot t) + B \cos (\sqrt \frac{g}{l} \cdot t)$$
Somit ist die Kreis-(eigen)-Frequenz $\omega = \sqrt{\frac{g}{l}}$.
##### Lagrangian
$$L = \frac{1}{2}ml^2 \dot \theta^2 + mgl \cos(\theta) $$
$$ \frac{d}{dt} \frac{\partial L}{\partial \dot \theta} = \frac{\partial L}{\partial \theta}$$
$$ \Longleftrightarrow ml^2 \ddot \theta = -mgl \sin(\theta)$$
$$\Longleftrightarrow  \frac{d^2s}{dt} = -\frac{g}{l}\sin(s)$$


#wellen 