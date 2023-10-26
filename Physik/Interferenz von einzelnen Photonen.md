Unter Interferenz von einzelnen Photonen versteht man die [[Interferenz]] welche durch [[Superpositionsprinzip|Superposition]] bei z.B. einem [[Doppelspalt]] auftritt. Hierbei fliegt ein einzelnes Photon durch beide Öffnungen des Doppelspaltes und interferiert somit mit sich selber. Dies wird dadurch deutlich, das ein Detektor an einem Spalt, den Kollaps der Wellenfunktion auslöst und sich kein nun kein Interferenzmuster bildet. 

![[Pasted image 20231023201845.png]]

Die Interferenz von einzelnen Photonen lässt sich auch anhand eines <a href=https://de.wikipedia.org/wiki/Mach-Zehnder-Interferometer>Mach-Zehnder-Interferometer (Wkpd)</a> wahrnehmen. Hierbei wird ein Photon durch einen Strahlenteiler auf zwei Spiegel geleitet, diese Spiegel leiten das Photon nun auf einen weiteren Strahlenteiler. Wird das System richtig aufgebaut, kann durch eine z.B. Phasendifferenz konstruktive und destruktive in den jeweiligen Ausgängen des Strahlenteilers erzeugt werden. Hierbei interferiert das Photon mit sich selbst und befindet sich somit wieder in einer Superposition, welche aus den beiden Wegen besteht. Blockiert man einen der beiden Wege, so lässt sich dieser Effekt nicht wahrnehmen und es kommen in beiden Ausgängen jeweils gleich wahrscheinlich Photonen an.

![[Pasted image 20231024160724.png]]

Dieser Effekt kann ausgenutzt werden um einen <a href=https://en.wikipedia.org/wiki/Elitzur%E2%80%93Vaidman_bomb_tester>Elitzur–Vaidman bomb tester</a> zu bauen.


## Mathe ist toll (unvollständig)
Die mathematische Beschreibung eines Mach-Zehnder-Interferometer, lässt sich auf die Beschreibung von Strahlenteilern reduzieren. Hierbei lässt sich zwischen klassischen Strahlenteilern und quantenmechanischen Strahlenteilern unterscheiden. 

#### Klassischer Strahlenteiler
Ein klassischer Strahlenteiler hat zwei Eingänge und zwei Ausgänge, hierbei treffen die E-Felder $E_a$ und $E_b$ auf den Strahlenteiler, diese werden von dem Strahlenteiler zu $E_c$ und $E_d$ ''geteilt''. Hierbei lässt sich feststellen, das dies linear passiert und sich somit als lineare Transformation darstellen lässt:
$$\begin{pmatrix} E_c\\E_d \end{pmatrix} = \begin{pmatrix} r_{ac} & t_{bc}\\t_{ad} & r_{bd} \end{pmatrix} \begin{pmatrix} E_a\\E_b \end{pmatrix}$$
Hier wird der Strahlenteiler als Matrix dargestellt, wobei die $r$ Koeffizienten den Reflexionsgrad und die $t$ Koeffizienten den Transmissionsgrad darstellen. Diese Werte sind abhängig von dem Strahlenteiler. Damit der Strahlenteiler die Energieerhaltung erfüllt, muss folgendes gelten:
$$\left|\begin{pmatrix} E_c\\E_d \end{pmatrix}\right| = \left|\begin{pmatrix} E_a\\E_b \end{pmatrix}\right|$$
Beziehungsweise:
$$|E_c|^2+|E_d|^2 = |E_a|^2+|E_b|^2$$
Hieraus ergibt sich:
$$|r_{ac}|^2 + |t_{ad}|^2 = 1$$
und
$$|r_{bd}|^2 + |t_{bc}|^2 = 1$$
Diese Aussagen lassen sich damit beschreiben, dass ein E-Feld, welches durch $a$ oder $b$ auf den Strahlenteiler trifft genauso viel betragen muss wie die summe von den E-Feldern welche aus $c$ und $d$ austreten (der Strahlenteiler kann keiner Energie erzeugen oder vernichten). Dies impliziert, folgendes:
$$r_{ac}t_{bc}^* +t_{ad}r_{bd}^* = 0$$
Somit gilt auch:
$$ M^{\dagger}M = I$$
Wobei $M$ die Matrix des Strahlenteilers ist. Hieraus lässt sich einfach erkennen, dass es sich bei $M$ um eine Unitäre Matrix handeln muss, um die Energieerhaltung zu erfüllen. Ein 50:50 Strahlenteiler kann z.B. folgenderweise dargestellt werden:
$$M=\frac{1}{\sqrt{2}}\begin{pmatrix}1 & 1\\1 & -1\end{pmatrix}$$


#quantenphysik 