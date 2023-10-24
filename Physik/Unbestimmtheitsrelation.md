Die Heisenbergsche Unbestimmtheitsrelation (auf Ort und Impuls bezogen) besagt, dass das Produkt der Standardabweichungen von Position und Impuls größer als $\frac{\hbar}{2\pi}$ ist.
$$\sigma_x \sigma_p \geq \frac{\hbar}{2} = \frac{h}{4\pi}$$
Die Unbestimmtheitsrelation(en) sind direkte folgen der Cauchy-Schwarz Ungleichung.

## Mathe
Für jede physikalische messbare Quantität $A$ mit einem Operator $\hat A$ ist die Varianz gegeben durch:
$$\sigma^2_A = \braket{(\hat A - \braket{A}) \Psi|(\hat A - \braket{A}) \Psi} = \braket{f|f}$$
wobei $f := (\hat A - \braket{A}) \Psi$. Nun gilt wegen Cauchy-Schwarz folgendes:
$$\sigma_A^2\sigma_B^2 = \braket{f|f}\braket{g|g} \geq |\braket{f|g}|^2$$
### Lemma I
Für jede komplexe Zahl gilt (Dreiecks Ungleichung):
$$|z|^2 \geq \Im (z)^2$$
somit gilt:
$$|z|^2 \geq \left[\frac{1}{2i} (z - z^*)\right]^2$$
Durch einsetzen von Lemma I in Mathe, erhalten wir:
$$\sigma_A^2\sigma_B^2 \geq |\braket{f|g}|^2 \geq \left[ \frac{1}{2i}(\braket{f|g} - \braket{g|f})\right]^2$$
Nun gilt:
$$\braket{f|g} = \braket{(\hat A - \braket{A})\Psi| (\hat B - \braket{B})\Psi} = \braket{\Psi| (\hat A - \braket{A})(\hat B - \braket{B})\Psi}$$
Durch Umformung erhält man nun:
$$\braket{\Psi| \hat A \hat B \Psi} - \braket{B}\braket{\Psi|\hat A \Psi}- \braket{A}\braket{\Psi|\hat B \Psi} + \braket{A} \braket{B}\braket{\Psi|\Psi}$$
$$= \braket{\hat A \hat B} - \braket{B}\braket{A}-\braket{A}\braket{B}+\braket{A}\braket{B}$$
$$\Rightarrow \braket{f|g} = \braket{\hat A \hat B} - \braket{B}\braket{A}$$
Da wir jedoch in $\braket{f|g} - \braket{g|f}$ Interessiert sind fällt der letze Term weg:
$$\braket{f|g} - \braket{g|f} = \braket{\hat A \hat B} - \braket{\hat B \hat A} = \braket{[\hat A,\hat B]}$$
Somit lautet die generelle Unbestimmtheitsrelation:
$$\sigma_A^2\sigma_B^2  \geq \left[ \frac{1}{2i}(\braket{[\hat A,\hat B]})\right]^2$$
Für $[\hat x, \hat p] = i\hbar$ erhält man:
$$\sigma_x^2\sigma_p^2  \geq \left[ \frac{1}{2i}(i\hbar)\right]^2 = \left( \frac{\hbar}{2}\right)^2$$
Und somit ergibt sich bekante form:
$$\sigma_x \sigma_p \geq \frac{\hbar}{2} = \frac{h}{4\pi}$$
#quantenphysik 