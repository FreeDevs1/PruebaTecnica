# 🛸 Who the Schwifty?

**Una app iOS de Rick and Morty desarrollada con SwiftUI**  
Prueba técnica por **Noguerón Méndez José Antonio**

---

## 📱 Descripción

**Who the Schwifty?** es una aplicación iOS construida con SwiftUI que consume la [API oficial de Rick and Morty](https://rickandmortyapi.com/). La app permite explorar personajes, buscar, filtrar por estado (vivo, muerto, desconocido), marcar favoritos con persistencia local y proteger el acceso con biometría (Face ID o Touch ID). También se enfoca en ofrecer una interfaz animada, fluida y moderna.

---

## ✨ Funcionalidades

- **Búsqueda** en tiempo real por nombre de personaje  
- **Favoritos persistentes** con almacenamiento local (`@AppStorage`)  
- **Filtros por estado** (Vivo, Muerto, Desconocido)  
- **Detalle de personajes** con imagen, estado, especie y ubicación  
- **Autenticación biométrica** para proteger la sección de favoritos  
- **Animaciones y UI fluida** usando `.matchedGeometryEffect`, `.snappy` y más  
- **Indicadores de carga** tipo *skeleton* para una mejor UX  
- **Caching local** de personajes para evitar recargas innecesarias  
- **Carga paginada** de la API, hasta obtener todos los personajes disponibles  

---

## 🛠️ Tecnologías usadas

- ✅ **SwiftUI** – Framework principal para la UI declarativa
- ✅ **Combine** – Gestión de estados reactivos
- ✅ **Kingfisher** – Para manejo de imágenes con cache
- ✅ **LocalAuthentication** – Face ID / Touch ID
- ✅ **UserDefaults (`@AppStorage`)** – Persistencia simple de datos
- ✅ **Rick and Morty API** – Fuente de los personajes

---

## 🧠 Arquitectura

- MVVM (`CharactersViewModel`, `Character` model, etc.)
- Separación de responsabilidades (servicios de red, vista, lógica de UI)
- Composición basada en Views reusables
- Persistencia local de favoritos y personajes usando `JSONEncoder/Decoder`

---

## 🔐 Requisitos

- iOS 17.0+
- Xcode Beta+
- Conexión a internet (solo en primer uso)

---

## 🚀 Instalación y ejecución

1. Clona el repositorio:
   ```bash
   git clone https://github.com/tuusuario/who-the-schwifty.git
