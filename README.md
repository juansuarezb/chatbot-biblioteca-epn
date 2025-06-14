#  BiblioEPN – Chatbot Inteligente para la Biblioteca de la Facultad de Sistemas

Este proyecto consiste en la implementación de un agente conversacional que permite a los estudiantes de la **Escuela Politécnica Nacional buscar libros disponibles en la biblioteca de la Facultad de Sistemas.** Se trata de un prototipo funcional desarrollado en Google Colab, que utiliza procesamiento de lenguaje natural (NLP) para entender consultas por título, autor o temática.

---

## Objetivo del proyecto

Desarrollar un agente inteligente que permita a los estudiantes consultar la disponibilidad de libros en la biblioteca, mediante lenguaje natural. Este chatbot se presenta como una solución a la falta de herramientas conversacionales que faciliten el acceso rápido a la información bibliográfica en la EPN.

---

## Planteamiento del problema

Como estudiantes, identificamos que muchas veces necesitamos buscar libros por tema o autor sin saber cómo navegar adecuadamente el sitio web de la biblioteca. Además, no existe actualmente un asistente conversacional que nos guíe o sugiera recursos académicos. Este chatbot busca resolver esa necesidad.

---

## 👥 Población objetivo

- Estudiantes de la EPN (principalmente de la Facultad de Sistemas)
- Docentes que desean recomendar libros a sus alumnos
- Personal administrativo de bibliotecas

---

## 🧾 Información que brinda el chatbot

- Búsqueda de libros por **título**
- Búsqueda de libros por **autor**
- Búsqueda de libros por **temática o área**
- Información sobre **servicios, horarios y contacto de la biblioteca**

---

## 🔧 Herramientas utilizadas

- 🧠 **Google Colab**
- 🐍 **Python 3**
- 📚 **NLTK** para procesamiento de lenguaje natural
- 🔍 **Web Scraping (BeautifulSoup)** para obtener información desde https://biblioteca.epn.edu.ec/
- 💬 Diseño propio de prompts y flujos conversacionales

---

## 📊 Casos de uso

1. Buscar libro por título
2. Buscar libro por autor
3. Buscar libro por temática
4. Consultar horarios y contacto de la biblioteca
5. Administrador: Cargar o actualizar datos
6. Administrador: Validar funcionamiento del chatbot

📌 El diagrama de casos de uso se encuentra en el archivo [`casos_de_uso.md`](casos_de_uso.md).

---

## 🖼 Diagrama de interacción

- El usuario envía una consulta por texto (ej. "¿Tienen libros sobre Inteligencia Artificial?")
- El chatbot interpreta la intención (por keyword o similaridad)
- Se busca en el conjunto de datos previamente extraído desde el portal de la biblioteca
- Se devuelve una lista de libros relevantes

---

## ⚙️ Instalación de dependencias (en Colab)

En la primera celda del notebook se deben instalar:

```python
!pip install nltk beautifulsoup4 requests
