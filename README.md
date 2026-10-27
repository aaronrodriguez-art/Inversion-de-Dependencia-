# Inversion-de-Dependencia-
Principio Inversion de Dependencia de SOLID

Este principio se aplica haciendo que las clases dependan de abstracciones y no de implementaciones concretas:

- Tenemos una clase abstracta llamada `EnvioRecibo` que funciona como la interfaz general.
- En la clase `AdmProducto`, el método `Compra` recibe un puntero de tipo `EnvioRecibo` (`EnvioRecibo *enviorecibo`) en lugar de amarrarse a clases específicas como correo o app.
- Las clases hijas (`EnviarEmail` y `EnviarApp`) heredan de esa abstracción para cumplir con el envío.

