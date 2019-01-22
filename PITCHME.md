# Pruebas unitarias con JUnit

---

## ¿Qué son las pruebas unitarias?
Las pruebas unitarias pretenden probar el comportamiento correcto de las clases de manera aislada.

Esto significa que se prueba la clase aislándola de su interacción con otras clases.

+++

### Principios FIRST para la escritura de pruebas unitarias
**F**: Fast, los test se han de ejecutar rápidamente.

**I**: Isolated, los test se realizan sobre una clase sin interacción con otras.

**R**: Repeatable, el orden de ejecución de los test no debe influir en el resultado final.

**S**: Self-validating, los test se han de ejecutar de modo automático.

**T**: Timely, se han de crear al mismo tiempo que el software que se está creando.

---

## El framework JUnit

Existen frameworks para realizar pruebas unitarias para prácticamente cualquier lenguaje de programación.

En el caso de Java podemos incluso elegir entre varias opciones.

Una de ellas es JUnit, puede que la más consolidada.

[JUnit](http://www.junit.org/) JUnit este es el enlace a la página principal de este framework.

+++

### Crear pruebas unitarias en Eclipse

Lo primero que hay que saber es que JUnit ya está integrado en Eclipse. Cuando te descargas Eclipse también te estás descargando JUnit y los plug-ins de Eclipse para el trabajo con este framework.

+++
### Crear pruebas unitarias en Eclipse
Supongamos que queremos crear un test para esta clase.

    public class Aritmetica {
        private float ultimoResultado;
        public float suma(float primerSumando, float segundoSumando) {
            return ultimoResultado = primerSumando + segundoSumando;
        }
        public float resta(float minuendo, float sustraendo) {
            return ultimoResultado = minuendo - sustraendo;
        }
        public float multiplicacion(float primerFactor,
            float segundoFactor) {
            return ultimoResultado = primerFactor * segundoFactor;
        }
        public float division(float dividendo, float divisor) {
            return ultimoResultado = dividendo / divisor;
        }
    	public float getUltimaResultado() {
        	return ultimoResultado;
    	}
    }
    
+++
### Crear pruebas unitarias en Eclipse
Haz click con el botón derecho del ratón sobre el paquete donde quieres añadir la nueva clase de prueba.

En el menú emergente selecciona New → JUnit Test Case se abrirá una ventana como la siguiente.
![New Junit Test](/home/joadelvia/Descargas/creacionTestCase.png  "New Junit Test")
