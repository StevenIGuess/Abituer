Ein quantenmechanisches System lässt sich Mathematisch durch eine Wellenfunktion beschreiben. Hierfür wird meistens der griechische Buchstabe Psi ($\psi$) verwendet. Die Wellenfunktion ist normalerweise mehrdimensional und hängt von Ort und Zeit ab. Somit lässt sich diese meistens durch $\Psi(\vec{r}, t)$ beschreiben. Hierbei ist $\vec r$ ein $n$ dimensionaler Vektor welcher die Position angibt. Es wird unterschieden zwischen der Zeit-_un_-abhängigen Wellenfunktion $\psi(\vec r)$
und der Zeitabhängigen Wellenfunktion $\Psi(\vec r, t)$. Diese lassen sich durch die Schrödinger Gleichung lösen:
Zeitabhängig:
$$i\hbar \frac{\partial \Psi}{\partial t} = - \frac{\hbar^2}{2m}\frac{\partial^2\Psi}{\partial x^2} + V\Psi$$
Falls diese Gleichung durch Trennung der Veränderlichen gelöst werden kann ergibt sich nun die Zeit-_un_-abhängige Schrödinger Gleichung:
$$\Psi(\vec r, t) = \psi(\vec r)\varphi(t)$$
$$-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} + V \psi = E \psi$$
$$\varphi(t) = e^{\frac{-iEt}{\hbar}}$$
Somit reicht es die Schrödinger Gleichung für Trennbare Systeme, anhand der Zeit-_un_-abhängigen Schrödinger Gleichung zu Lösen um eine Lösung für alle $t$ zu erhalten, da $\varphi$ trivial ist. Da es sich bei der Wellenfunktion um eine komplexe Funktion handelt, ist die Interpretation dieser etwas komplex. Laut der statistischen gibt der Ausdruck $\braket{\Psi|\hat A|\Psi}$ den Erwartungswert $\braket{\hat A}$, wobei $\hat A$ ein Hermetische Operator ist, welcher eine physikalische Größe darstellt. Der Operator $\hat x = x$ stellt z.B. die Position da, somit ist $\braket{\Psi|\hat x | \Psi}$ der Erwartungswert der Position. Der Ausdruck $|\Psi|^2$ gibt die Wahrscheinlichkeit, dass das untersuchte Teilchen sich an Position $\vec r$ befindet. Somit gibt folgender Ausdruck den Erwartungswert für den Impuls:
$$\braket{\hat p} = \braket{\Psi|\hat p |\psi} = \int_{-\infty}^{\infty} \Psi^* (-i\hbar\frac{\partial \Psi}{\partial x})dx$$

-> Müll, warum ist das im Abitur lol

#quantenphysik 