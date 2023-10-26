Das lineare Kraftgesetz besagt, dass eine Lineare Kraft (wie z.B. Hookesche Federn) in einer harmonischen Schwingung resultieren. Eine lineare Kraft bedeutet in diesem Kontext folgendes:
$$ F(x) = kx$$
Somit ist die Kraft $F$ proportional zur Auslenkung ($F \propto x$). Aus dem ersten N. Gesetz folgt:
$$ F = m\cdot a \Longleftrightarrow a = \frac{F}{m} = \frac{kx}{m}$$
Durch Substitution $\rho = -\frac{k}{m}$ erhält man:
$$ a = -\rho x$$
bzw.
$$\frac{d ^2x}{dt^2} = -\rho x$$
Die Lösung für diese Gleichung ist (trivial, (Wolfram Alpha)): 
$$ x(t) = A\sin(\sqrt \rho \cdot t) + B \cos (\sqrt \rho \cdot t)$$
Dies ist die Wellengleichung für z.B. ein Federpendel mit $\rho = \frac{D}{m}$, wobei $D$ die Federkonstante ist. Die Koeffizienten $A$ und $B$ lassen sich durch Grenzbedingungen ermitteln. Gilt z.B. $x(0) = 0$, impliziert dies $B = 0$ und $A = x_{max}$ (Amplitude).

#wellen 