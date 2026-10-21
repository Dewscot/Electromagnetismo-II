---
tags:
  - electromagnetismo-ii
  - certamen-2
  - inductancia
estado: en-estudio
fuente: "Contenido 4.1 510238 - Inductancia_EnergíaB, diapositivas 1–8"
---


> [!abstract] Pregunta física
> ¿Qué sucede cuando cambia la corriente en un circuito que genera su propio campo magnético?

## 1. Idea física

La corriente eléctrica $i(t)$ que atraviesa una bobina produce un campo magnético $\mathbf B$. Si la corriente cambia con el tiempo, también puede cambiar el flujo magnético que atraviesa las espiras. Por la ley de Faraday-Lenz, aparece una **fem autoinducida** que se opone a esa variación.

**Ojo:** la autoinducción se opone al *cambio* de corriente, no necesariamente al sentido que tenga la corriente.

## 2. Desde la ley de Faraday a la inductancia

El flujo magnético a través de **una espira** es

$$
\Phi_B=\int_S\mathbf B\cdot d\mathbf A.
$$

Para una bobina de $N$ espiras que enlazan el mismo flujo, el enlace de flujo es $\lambda=N\Phi_B$. La ley de Faraday-Lenz es

$$
\mathcal E_{\mathrm{ind}}=-\frac{d\lambda}{dt}=-N\frac{d\Phi_B}{dt}.
$$

En un circuito lineal de geometría fija, $\lambda$ es proporcional a $i$ y se define la **autoinductancia** $L$ mediante

$$
\boxed{\lambda=Li}\qquad\Longrightarrow\qquad\boxed{L=\frac{N\Phi_B}{i}}.
$$

Si $L$ es constante:

$$
\boxed{\mathcal E_{\mathrm{ind}}=-L\frac{di}{dt}}.
$$

El signo negativo expresa la ley de Lenz: la fem inducida se opone a la variación que la produce. Cuando se usa la **convención pasiva de signos**, la caída de tensión del inductor se escribe

$$
\boxed{v_L=L\frac{di}{dt}}.
$$

Estas expresiones no se contradicen: se refieren a convenciones de signos distintas.

## 3. Ejemplo fundamental: solenoide largo

Consideremos un solenoide ideal, largo, de $N$ espiras, longitud $\ell$, sección transversal $A$ y núcleo de aire o vacío. Despreciando efectos de borde:

$$
B\simeq \mu_0\frac{N}{\ell}i.
$$

El campo es aproximadamente uniforme y paralelo a la normal de las espiras, por lo que

$$
\Phi_B=BA=\mu_0\frac{N}{\ell}iA.
$$

Con $L=N\Phi_B/i$ obtenemos

$$
\boxed{L=\mu_0\frac{N^2 A}{\ell}}.
$$

**Interpretación:** en este modelo, la inductancia depende de la geometría y de la permeabilidad magnética, no del valor instantáneo de la corriente. Si el medio lineal tiene permeabilidad $\mu$, se reemplaza $\mu_0$ por $\mu$.

## 4. Comprobaciones y casos límite

- **Unidades:** $[L]=\mathrm{Wb/A}=\mathrm{V\,s/A}=\mathrm H$ (henry).
- **Corriente constante:** $di/dt=0$ implica $\mathcal E_{\mathrm{ind}}=0$, aunque $B$ y la energía magnética puedan ser distintos de cero.
- **Mayor número de espiras:** si se duplica $N$, manteniendo constantes $\ell$, $A$ y el material del solenoide ideal, $L$ se cuadruplica.
- **Mayor rapidez de cambio:** a $L$ fija, una variación más rápida de $i$ da una fem inducida de mayor módulo.

## 5. Qué debo poder deducir sin consultar

- [ ] Explicar por qué una corriente variable puede producir una fem en el mismo circuito.
- [ ] Partir de $\mathcal E=-d\lambda/dt$ y obtener $\mathcal E=-L\,di/dt$ bajo sus hipótesis.
- [ ] Distinguir la fem autoinducida de la tensión $v_L$ con convención pasiva.
- [ ] Deducir $L=\mu_0 N^2 A/\ell$ para un solenoide ideal.
- [ ] Interpretar el caso $di/dt=0$ y comprobar unidades.

## 6. Preguntas de recuperación activa (sin mirar)

1. Si una corriente atraviesa una bobina y permanece constante, ¿existe campo magnético? ¿Existe fem autoinducida?
2. Si aumenta el ritmo de cambio de la corriente, pero no cambia $L$, ¿qué ocurre con $|\mathcal E_{\mathrm{ind}}|$?
3. ¿Por qué al duplicar las espiras de un solenoide largo ideal la inductancia se multiplica por cuatro?

## Conexión con las secciones siguientes

La relación $v_L=L\,di/dt$ permitirá construir las EDO de [[01 - Oscilaciones LC]]. Antes revisaremos el balance energético en [[00.2 - Energia magnetica]]. La energía almacenada en un inductor se desarrolla **en la siguiente nota**, no en esta.

---

**Fuente principal:** presentación del profesor, *Contenido 4.1 — Inductancia y Energía B*, diapositivas 1–8. El modelo del solenoide se estudia como ejemplo idealizado.
