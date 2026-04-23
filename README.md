[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=FernandaAntunez/Practica2GD&project=https://github.com/FernandaAntunez/Practica3GD)]

# Práctica 3: Liberación controlada de fármacos por hidrogeles

## Información de la estudiante
Fernanda Antunez \[22211745]; L22211745@tijuana.tecn.mx

Gemelos Digitales

Ingeniería Biomédica

## Docente
Dr. Paul Antonio Valle Trujillo; paul.valle@tectijuana.edu.mx

Departamento de Ingeniería Eléctrica y Electrónica, Tecnológico Nacional de México/IT Tijuana, Blvd. Alberto Limón Padilla s/n, Tijuana, C.P. 22454, B.C., México.

## Descripción de la asignatura
La asignatura de Gemelos Digitales forma parte del plan de estudios de la carrera en Ingeniería Biomédica con la siguiente competencia general del curso: Formula el gemelo digital a través de datos experimentales para el desarrollo estrategias de control mediante teorías de sistemas dinámicos no lineales y la experimentación in silico. Esta asignatura pretende aportar al perfil del Ingeniero Biomédico la capacidad de realizar investigación científica en el área de Biología de Sistemas con la finalidad de dirigir y participar en equipos de trabajo interdisciplinarios en contextos nacionales e internacionales, así como de proporcionar soluciones informáticas para resolver problemas en el campo de la Ingeniería Biomédica con ética profesional.

En el contexto de sistemas dinámicos que describen sistemas biológicos o fisiológicos, el modelizado in silico es una extensión lógica de la experimentación in vitro controlada, es el resultado natural del gran aumento de la potencia computacional disponible a un costo que disminuye continuamente, combinando las ventajas de la experimentación in vivo e in vitro, sin someterse a las consideraciones éticas y la falta de control asociadas con los experimentos in vivo. A diferencia de los experimentos in vitro, que existen de forma aislada, los modelos in silico permiten incluir un conjunto prácticamente ilimitado de variables y parámetros, lo que hace que los resultados sean más aplicables en problemas del mundo real. La experimentación in silico ha dado lugar al paradigma denominado como "gemelos digitales" (en inglés digital twins); en esencia, los gemelos digitales son una réplica o representación digital de un proceso o sistema del mundo real, donde por replica se refiere a un modelo computacional desarrollado con base en datos experimentales y características especiales que le permiten conectar lo físico con lo virtual con el propósito de mejorar el rendimiento de un sistema, detectar y prevenir fallas, y realizar predicciones sobre su respuesta ante diferentes estímulos o escenarios de operación; una definición más formal establece que: un gemelo digital es un conjunto de modelos adaptativos que emulan el comportamiento de un sistema físico en un sistema virtual obteniendo datos en tiempo real para actualizarse a lo largo de su ciclo de vida; replica al sistema físico para predecir fallas y oportunidades de cambio, prescribir acciones en tiempo real para optimizar y/o mitigar eventos inesperados observando y evaluando el perfil operativo del sistema. En el campo particular de la Biología de Sistemas, un gemelo digital se presenta como un algoritmo o conjunto de algoritmos computacionales desarrollados con base en modelos mecanicistas de un organismo vivo, esto con el objetivo de emular su fisiología para ilustrar su dinámica en el corto y en el largo plazo, así como predecir su respuesta a diferentes estímulos endógenos y exógenos.

## Objetivo y descripción del sistema
Determinar la tasa de liberación del hidrogel N36 2MBA3 con base en los datos experimentales de la siguiente figura. <img width="725" height="576" alt="image" src="https://github.com/user-attachments/assets/e02017e1-977b-406b-bc7e-d6953d66a6ce" />


      Ecuación de Peppas: $x(t) = k t^n$ ...(1)
      Farmacocinética de primer orden: $x(t) = \beta(1 - e^{-kt})$ ...(2)
      Eureqa: $x(t) = \frac{p_1 t}{p_2 + t}$ ...(3)
      Eureqa EDO=  $\dot{x} = p_1 - p_2 x$ ...(4)

La descripción de cada ecuación del sistema se realiza a continuación. Primero, se observa en la estructura de la Ecuación (1) que el transporte de masa en la matriz polimérica se rige por la ley de potencia de Korsmeyer-Peppas, donde $k$ es una constante que incorpora las características estructurales del hidrogel y el exponente $n$ define el mecanismo de difusión (Fickiano o no Fickiano). En la Ecuación (2), el sistema describe una cinética de primer orden donde la liberación es proporcional a la cantidad de fármaco remanente; aquí $\beta$ representa la concentración máxima alcanzable en el equilibrio y $k$ la constante de velocidad de liberación.Por otro lado, la Ecuación (3) describe el crecimiento de la fracción liberada mediante un modelo de saturación tipo Michaelis-Menten (o Langmuir), donde el parámetro $p_1$ establece la capacidad de carga máxima del sistema y $p_2$ representa la constante de semisaturación, indicando el tiempo necesario para alcanzar la mitad de la liberación total.Finalmente, la Ecuación (4) presenta el modelo en su forma diferencial (EDO), la cual describe la tasa de cambio instantánea de la liberación ($\dot{x}$). En esta estructura, el término $p_1$ actúa como una tasa de entrada constante o flujo de liberación inicial, mientras que el término $-p_2x$ representa la resistencia o el freno del sistema a medida que se acerca al equilibrio, estableciendo una competencia dinámica entre la fuerza impulsora y la saturación del medio.


Palabras clave: Cinética de Liberación; Regresión No Lineal:; Modelado Estocástico; Simulaciones Numéricas; Solución de EDOs.

## Actividades a realizar
1. Cuaderno computacional de MATLAB
2. Análisis matemático
3. Generación de resultados gráficos

## Lista de archivos incluidos en el repositorio
1. Cuaderno computacional de MATLAB [.mlx].
2. Imágenes de las simulaciones [.pdf].
3. Análisis matemático [.pdf].

## Referencias
\[1] P. A. Valle, Syllabus para Gemelos Digitales, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México, 2025. Permalink: https://biomath.xyz/course/

\[2] Itik, M., & Banks, S. P. (2010). Chaos in a three-dimensional cancer model. international Journal of bifurcation and chaos, 20(01), 71-79. https://doi.org/10.1142/S0218127410025417

\[3] Bryan, Kurt. Differential equations: A toolbox for modeling the world. Simiode, 2022. Permalink: https://www.simiode.org/resources/8307 
