# Generador de Cadenas con Gramática Numérica

Este proyecto consiste en una simulación animada que valida cadenas numéricas basadas en una gramática libre de contexto,
inspirada en el concepto de Máquina de Turing.

### Objetivo

Permitir al usuario ingresar cadenas como `123`, `-45` o `0` y visualizar paso a paso su derivación conforme a una gramática definida.
En caso de ser una cadena inválida, se mostrará un mensaje de advertencia.

### Gramática utilizada

```ebnf
Numero → Signo NumeroSinSigno
Signo → '-' | λ
NumeroSinSigno → '0' | DigitoNoCero Digitos
Digitos → Digito Digitos | λ
Digito → '0' | DigitoNoCero
DigitoNoCero → '1' | '2' | ... | '9'
```

### Cómo usar

1. Abre el archivo `maquina_turing_gramatica_autor.html` en tu navegador.
2. Escribe una cadena como `123`, `-50`, `0`.
3. Presiona el botón **"Validar y Mostrar Derivación"**.
4. Observa la animación paso a paso del análisis.

### Estructura del proyecto

```
.
├── maquina_turing_gramatica_autor.html
└── README.md
```

Presentado por **Dilsa Barrientos**

---

Proyecto académico basado en Teoria de Lenguajes y Laboratorio - UdeA  
