Der lineare Potenzialtopf ist eine Potentialverteilung $V(x)$, welche häufig als vorzeige Beispiel für die Schrödinger Gleichung und Quantenmechanik verwendet wird. Weiterführend haben ähnliche Potenzialverteilungen Anwendung in der Technik. Die Verteilung ist folgendermaßen definiert:
$$V(x) = \left\{\begin{array}{lr}0, &  0 \leq x \leq l\\\infty, & \text{sonst }\end{array}\right .$$
Nun muss die Schrödinger Gleichung für $V$ gelöst werden:
$$i\hbar\frac{\partial \Psi}{\partial t} = -\frac{\hbar^2}{2m} \frac{\partial^2\Psi}{\partial x^2} + V\Psi$$
Da $V$ nicht von der Zeit $t$ abhängt, lässt sich diese Gleichung durch Trennung der Variablen folgendermaßen lösen:
$$\Psi(x,t) = \psi(x)\varphi(t)$$
$$\Longleftrightarrow \frac{\partial \Psi}{\partial t} = \frac{d\varphi}{dt} \psi \,\,\,\,,\,\,\,\,\frac{\partial^2 \Psi}{\partial x^2} = \frac{d^2\psi}{dx^2}\varphi$$
Durch einsetzen in die Schrödinger Gleichen erhält man folgendes:
$$i\hbar \frac{d\varphi}{dt} \psi = -\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2}\varphi + V\psi\varphi$$
Teil man nun durch $\varphi\psi$ resultiert dies in:
$$\frac{i\hbar}{\varphi} \frac{d\varphi}{dt} = -\frac{\hbar^2}{2m\psi}\frac{d^2\psi}{dx^2} + V$$
Da beide teile unabhängig voneinander sind müssen beide konstant sein, somit lässt sich die Trennungs-konstante $E$ einführen:
$$\frac{i\hbar}{\varphi} \frac{d\varphi}{dt} = E \,\,\,\, \Longleftrightarrow\,\,\,\, \frac{d\varphi}{dt} = \frac{E}{i\hbar}\varphi$$
$$-\frac{\hbar^2}{2m\psi}\frac{d^2\psi}{dx^2} + V = E\,\,\,\, \Longleftrightarrow\,\,\,\, -\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} + V\psi = E\psi$$
Die erste Gleichung ist Trivial:
$$\varphi = Ce^{-iEt /\hbar}$$
Das $C$ wird in $\psi$ aufgenommenen. Die zweite Gleichung stellt die Zeit-_un_-abhängige Schrödinger Gleichung dar:
$$\hat H \psi = E \psi$$
Außerhalb des Bereiches $[0,l]$ gilt $V = \infty$ somit kann sich hier kein Teilchen befinden. Innerhalb des Bereiches gilt $V=0$, durch einsetzen in die Zeit-_un_-abhängige Schrödinger Gleichung erhält man:
$$-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} = E\psi$$
Definiert man nun $k = \frac{\sqrt{2mE}}{\hbar}$, lässt sich einfach erkennen:
$$ \frac{d^2\psi}{dx^2} = -k^2\psi$$
Die Lösung für diese Gleichung ist bekannt:
$$\psi = A\sin(kx)+ B\cos(kx)$$
Da $\psi$ jedoch stetig sein muss gilt $\psi (0) = 0$, deswegen gilt $B = 0$, somit ergibt sich:
$$\psi = A\sin(kx)$$
Die zweite Randbedingung besagt nun, dass $\psi(l) = 0$, damit dies erfüllt ist muss:
$$kl = m, \,\,\,\, m\in \{\pm \pi, \pm2\pi,\pm3\pi,...\} $$
Es gilt $\sin(-x) = -\sin(x)$ somit kann das minus in $A$ aufgenommen werden. Die Erlaubten Energie sind nun gegeben durch:
$$ k_n = \frac{n \pi}{l},\,\,\,\,n\in\mathbb{N}$$
$$ \Longleftrightarrow \frac{\sqrt{2mE}}{\hbar} = \frac{n\pi}{l}$$
$$ \Longleftrightarrow E_n = \frac{(n\pi\hbar)^2}{2ml^2}$$
Nun muss $\psi$ anhand von $A$ genormt werden:
$$\int_0^a |\psi|^2 dx = \int_0^a |A|^2 \sin^2(kx)\, dx = 1$$
Dies impliziert, dass:
$$ |A|^2\frac{l}{2} = 1 \Longleftrightarrow A = \sqrt\frac{2}{l}$$
Somit lässt sich $\psi$ aufstellen:
$$ \psi_n(x) = \sqrt\frac{2}{l} \sin \left(\frac{n \pi}{l}x\right)$$
Kombiniert man nun $\psi$ und $\varphi$ erhält man die stationäreren Zustände des Teilchens:
$$ \Psi_n (x,t)  = \sqrt\frac{2}{l} \sin \left(\frac{n \pi}{l}x\right)e^{-i\frac{(n\pi)^2\hbar}{2ml^2}t}$$
Die allgemeinste Lösung ist jedoch eine Lineare Kombination aus den stationären Zuständen:  
$$  \Psi (x,t) = \sum_{n=1}^\infty c_n  \sqrt\frac{2}{l} \sin \left(\frac{n \pi}{l}x\right)e^{-i\frac{(n\pi)^2\hbar}{2ml^2}t}$$
Die Koeffizienten $c_n$ werden nun durch Fourieres Trick gegeben, dafür muss unter anderem $\braket{\Psi_n|\Psi_m} = \delta_{n,m}$ (hier wird angenommen, dass dies stimmt);
$$c_n = \sqrt\frac{2}{l} \int_0^a \sin \left(\frac{n \pi}{l}x\right) \Psi(x,0) dx$$
Somit ist für ein gegebenes $\Psi(x,0)$ die Lösung der Zeit-abhängigen Schrödinger Gleichung:
$$  \Psi (x,t) = \sum_{n=1}^\infty \left( \sqrt\frac{2}{l} \int_0^a \sin \left(\frac{n \pi}{l}x\right) \Psi(x,0)dx\right)  \sqrt\frac{2}{l} \sin \left(\frac{n \pi}{l}x\right)e^{-i\frac{(n\pi)^2\hbar}{2ml^2}t}$$

Please send help
#quantenphysik 