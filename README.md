# 💖 Calculador de Amor — Demo en GitHub Pages

Este repositorio contiene una demostración simple y moderna de un **Calculador de Amor**, creada para mostrar cómo funciona el widget online.  
La demo está creada con GitHub Pages y enlaza al sitio oficial:

👉 **Sitio completo:** https://calculardeamor.com  
👉 **Repositorio:** https://github.com/jaderenata5541-wq/Calculador-de-Amor  
👉 **Perfil del autor:** https://github.com/jaderenata5541-wq  

---

## ❤️ ¿Qué es el Calculador de Amor?

El **Calculador de Amor** es una herramienta divertida donde los usuarios pueden ingresar dos nombres y obtener un porcentaje de compatibilidad.  
La versión completa ofrece:

- ✔️ Cálculo rápido y automático  
- ✔️ Algoritmo divertido basado en coincidencias de nombres  
- ✔️ Interfaz atractiva y fácil de usar  
- ✔️ Resultados listos para compartir  

Puedes usar la versión completa aquí:  
👉 **https://calculardeamor.com**

---

## 🌟 Vista Previa del Calculador (Demo)

La siguiente demo está incluida en el archivo `public/index.html` del repositorio.

```html
<div style="max-width:430px;margin:auto;padding:20px;background:#fff;border-radius:15px;box-shadow:0 0 20px rgba(0,0,0,0.1);font-family:Arial;">
    <h2 style="text-align:center;color:#e91e63;">💘 Calculador de Amor</h2>

    <p style="text-align:center;color:#555;">Ingresa dos nombres y descubre la compatibilidad.</p>

    <input id="name1" type="text" placeholder="Tu nombre" 
        style="width:100%;padding:12px;border-radius:10px;border:1px solid #ccc;margin-bottom:10px;">

    <input id="name2" type="text" placeholder="Nombre de tu pareja" 
        style="width:100%;padding:12px;border-radius:10px;border:1px solid #ccc;margin-bottom:10px;">

    <button onclick="calcLove()" style="width:100%;padding:12px;background:#e91e63;color:white;border:none;border-radius:10px;font-size:16px;cursor:pointer;">
        Calcular Amor ❤️
    </button>

    <h3 id="result" style="text-align:center;margin-top:15px;color:#e91e63;"></h3>

    <script>
        function calcLove() {
            let n1 = document.getElementById("name1").value;
            let n2 = document.getElementById("name2").value;

            if(n1.trim() === "" || n2.trim() === ""){
                document.getElementById("result").innerHTML = "Por favor ingresa ambos nombres.";
                return;
            }

            let percentage = Math.floor(Math.random() * 41) + 60; // 60–100%
            document.getElementById("result").innerHTML = 
                "❤️ Compatibilidad entre <b>" + n1 + "</b> y <b>" + n2 + "</b>: <strong>" + percentage + "%</strong>";
        }
    </script>
</div>

