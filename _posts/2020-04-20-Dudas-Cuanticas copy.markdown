---
layout: post
title:  "Dudas Cuánticas"
date:   2019-10-19 18:55:14 +0200
categories: Quantum Mechanics
mathjax: true
comments: true
---
$$\newcommand{\ket}[1]{\vert#1\rangle}$$
$$\newcommand{\bra}[1]{\langle#1\vert}$$
$$\newcommand{\braket}[2]{\langle#1\vert#2\rangle}$$
$$\newcommand{\mvop}[3]{\langle#1\vert#2\vert #3\rangle}$$

1. **¿Qué pasa con los cuerpos negros?**
    : Los cuerpos negros emiten radiación electromagnética. A mayor temperatura del cuerpo, mayor es la frecuencia para la que la radiación emitida es máxima. Para frecuencias mayores, la radiación disminuye.
    
    Si tengo un cuerpo negro y lo voy calentando, las partículas se agitan y se mueven. Los electrones, en particular, resultan acelerados y emiten radiación electromagnética. Dentro de la cavidad del cuerpo negro, esta radiación está conformada por ondas estacionarias. Se cuenta el número de dichas ondas en la frecuencia $$\nu, \nu+d\nu$$ para ver cómo depende el número de ondas con la frecuencia. Definimos después la densidad de energía como:
    
    $$ \dfrac{\textrm{nº de ondas en el intervalo de frecuencias}\times \textrm{energía promedio de dichas ondas}}{\textrm{volumen}}$$
    
    Se llega a que la densidad de energía depende en un factor $$\nu^2$$, según la teoría clásica. De esta manera, se obtiene que para frecuencias altas (ultravioleta), los resultados experimentales no se parecen ni de lejos a lo hallado con la teoría. La teoría predice una divergencia y el experimento dice que se va a cero.
    
2. **¿Qué es la catástrofe ultravioleta?**
    
    
3. **¿Por qué cuantizar la energía en un cuerpo negro resuelve dicha catástrofe?**
    
    

4. **¿Por qué no se cae el electrón al núcleo?**
    : Porque no puede. En primer lugar, cuando estamos dentro de un átomo, la energía potencial que dicho electrón tiene es negativa. Esto quiere decir que el electrón está confinado, es decir, no puede salir del átomo libremente. ¿Por qué? Porque al ser negativa la energía, esto quiere decir que el aporte energético que hay que darle para desvincularlo del átomo es positivo, es decir, se requiere de energía para liberarlo. Pensar en la gráfica del potencial Coulombiano: para energías menores que cero, las regiones clásicamente permitidas son hasta cierto $$r>0$$, pero si la energía total es $$E\geq0$$ el electrón puede moverse libremente por todo el espacio.
    
    * **El electrón en el estado fundamental NO EMITE RADIACIÓN.** 
      : Si emitiera radiación, esta debería tener frecuencia $$\nu=\frac{\Delta E}{h}=\frac{E_{fund}-E'}{h}$$ pero es que no hay un estado con $$E'<E_{fund}$$ tal y como se sigue de la resolución de la ecuación de Schrödinger o de los postulados de Bohr. Por ello, el electrón no va a perder energía en forma de radiación.
    
      Pero esto sigue sin explicar que no caiga al núcleo, porque el hecho de que no radíe energía no implica que la partícula no pueda acercarse todo lo posible al núcleo. Al fin y al cabo, $$r<r_{Bohr}$$ es una región permitida para el átomo. Sí, esto es cierto, pero conforme nos acercamos al núcleo atómico, la energía potencial es proporcional a $$-\frac{1}{r}$$, y si $$r\to0$$ esta tiende a $$-\infty$$. En cambio, la energía cinética crece como $$\frac{1}{r^2}$$ cuando $$r>0$$, esto es, crece mucho más rápido que como decae la potencial. Así, *ganaría* la energía cinética del átomo y por ello no se quedaría en el núcleo.
    
      Además, el ppo. de incertidumbre nos dice que tampoco tiene mucho sentido plantearse esta cuestión de *caer al núcleo* porque al fin y al cabo, el electrón se comporta como una onda. De hecho, conforme más cerca del átomo estoy (más determinada la posición), más indeterminado el momento y por tanto, mayor incertidumbre en la energía cinética. En principio, se busca un equilibrio, el tamaño energéticamente más favorable. Para ello, ponemos $$E=T+V$$ como función del radio $$r$$ y derivamos con respecto a él, obteniéndose un mínimo de $$E$$ estable en $$r=r_{Bohr}$$.
    
      Consultar [Estabilidad de los átomos](https://mathoverflow.net/questions/119495/mathematical-proof-of-the-stability-of-atoms) para más información al respecto.
    
5. **Combinación que no presente desfase**
    : Que las constantes no sean complejas.
    
6. **¿Cuál es la paridad de los armónicos esféricos?**

7. **Why do we measure eignevalues?**
    : The answer to this question resides on the postulates of Quantum Mechanics. Let's say we perform an experiment in a Laboratory and we measure a certain property of a quantum system, for instance its energy, and we get a value $$E$$. Upon measurement, our wave function collapses into this particular state $$\ket{E}$$, and if we repeat our measurement we would still get the value $$E$$.
    
    We have postulated that to each observable magnitude corresponds a Hermitian operator. In this case, the Hamiltonian $$\hat{H}$$. That postulate also tells us that if we make the operator act on the state $$\ket{E}$$ we would get $$\hat{H}\ket{E}=E\ket{E}$$. That is, the energy we have measured is an eigenvalue of the operator because of the way we have defined Quantum Mechanics.

8. **Measuring vs Operators**
    : Measuring is not making the operator act on the wave function. Measuring is some physical experiment that takes place on a laboratory.
9. **¿Qué pasa si mido un estado con degeneración? ¿Se colapsa a un estado concreto o puede ser varios?**