# Sorteo de Amigos 🎉

Este proyecto es una aplicación web sencilla que permite agregar amigos a una lista y luego seleccionar aleatoriamente a uno de ellos. Su propósito es fortalecer habilidades en lógica de programación y manipulación del DOM con JavaScript.

## 🚀 Características

- Agregar nombres de amigos a una lista.
- Evitar duplicados en la lista.
- Mostrar la lista de amigos en la interfaz.
- Seleccionar aleatoriamente un amigo de la lista.

## 📋 Requisitos

- Un navegador web moderno (Chrome, Firefox, Edge, etc.).
- Conocimientos básicos de HTML, CSS y JavaScript.

## 📂 Estructura del Proyecto

El proyecto está compuesto por los siguientes archivos:

```
📁 proyecto-sorteo-amigos/
├── 📄 index.html  # Archivo principal con la estructura de la página
├── 📄 style.css   # Estilos de la aplicación
├── 📄 app.js      # Lógica en JavaScript para gestionar el sorteo
├── 📁 assets/     # Imágenes y recursos gráficos
```

## ⚙️ Instalación y Uso

1. Descarga o clona este repositorio en tu computadora:

   ```bash
   git clone https://github.com/tu_usuario/proyecto-sorteo-amigos.git
   ```

2. Abre el archivo `index.html` en tu navegador web.

3. Ingresa los nombres de los amigos en el campo de entrada y agrégalos a la lista.

4. Haz clic en el botón de sorteo para seleccionar un amigo al azar.

## 📌 Uso del Código

### 📌 Agregar un Amigo

```javascript
function agregarAmigo() {
    const inputAmigo = document.getElementById("amigo");
    const nombreAmigo = inputAmigo.value.trim();

    if (nombreAmigo === "") {
        alert("Por favor, inserte un nombre.");
        return;
    }
    
    if (amigos.includes(nombreAmigo)) {
        alert(`El nombre ${nombreAmigo} ya está en la lista.`);
        return;
    }

    amigos.push(nombreAmigo);
    inputAmigo.value = "";
    actualizarLista();
}
```

### 📌 Seleccionar un Amigo Aleatorio

```javascript
function sortearAmigo() {
    if (amigos.length === 0) {
        alert("No hay amigos en la lista para sortear.");
        return;
    }
    
    const indiceAleatorio = Math.floor(Math.random() * amigos.length);
    const amigoSorteado = amigos[indiceAleatorio];
    
    document.getElementById('resultado').innerHTML = `Amigo sorteado: <strong>${amigoSorteado}</strong>`;
}
```

## 🛠 Posibles Mejoras

- Agregar estilos CSS para mejorar la apariencia de la interfaz.
- Implementar almacenamiento en `localStorage` para persistir la lista de amigos.
- Permitir eliminar nombres de la lista.
- Agregar una opción para reiniciar la lista.

## 📜 Licencia

Este proyecto es de código abierto y se encuentra bajo la licencia MIT. Puedes usarlo y modificarlo libremente.

## ✉️ Contacto

Si tienes alguna pregunta o sugerencia, no dudes en contactarme a través de [apachecorios@outlook.com] o [apachecorios].

