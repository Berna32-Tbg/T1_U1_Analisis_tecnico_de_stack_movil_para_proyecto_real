# Reporte Técnico – Stack para App de Gestión de Citas Médicas

Este repositorio contiene el análisis y selección del stack de desarrollo para una aplicación móvil de gestión de citas médicas en Android e iOS.

---

## 1. Comparativa de Frameworks

- **Flutter**
  - Lenguaje: Dart  
  - Rendimiento: Muy alto (renderizado nativo con Skia)  
  - Curva de aprendizaje: Media (requiere aprender Dart)  
  - Comunidad: Amplia y activa  
  - Ejemplos de apps: Google Ads, BMW, Nubank  

- **React Native (Expo)**
  - Lenguaje: JavaScript/TypeScript  
  - Rendimiento: Alto (usa puente con componentes nativos)  
  - Curva de aprendizaje: Baja (JS/TS muy conocido)  
  - Comunidad: Muy amplia  
  - Ejemplos de apps: Instagram, Discord, Bloomberg  

- **Kotlin Multiplatform**
  - Lenguaje: Kotlin  
  - Rendimiento: Muy alto (código compartido, UI nativa)  
  - Curva de aprendizaje: Alta (conceptos multiplataforma)  
  - Comunidad: Creciente, más en entornos enterprise  
  - Ejemplos de apps: Netflix, VMware, Philips  

---

## 2. Selección de Lenguaje

**Elección final:** **TypeScript con React Native (Expo)**

**Justificación técnica:**
- Comunidad enorme y soporte multiplataforma.  
- Integración sencilla con librerías médicas (QR, notificaciones, almacenamiento).  
- Menor curva de aprendizaje y más desarrolladores disponibles.  
- Expo simplifica la configuración inicial y despliegue rápido.  

---

## 3. Entorno de Desarrollo

### Opción A: Android Studio (última versión estable)
- Instalar desde la web oficial.  
- Configurar SDK de Android y emuladores.  
- Instalar plugin de **React Native Tools**.  

### Opción B: Visual Studio Code (VS Code)
- Instalar VS Code.  
- Plugins recomendados:  
  - React Native Tools  
  - Expo Tools  
  - ESLint + Prettier  
  - TypeScript Language Features  

**Capturas incluidas en el PDF:**
1. Pantalla de instalación de VS Code.  
2. Configuración de plugins.  
3. Proyecto inicial con Expo (`npx create-expo-app citas-medicas`).  

---

## 4. Análisis de Hardware

La aplicación requiere:  
- **Cámara:** Escaneo de QR para confirmar citas o acceder a historial.  
- **Notificaciones push:** Recordatorios de citas y alertas médicas.  
- **Almacenamiento local (SQLite/AsyncStorage):** Historial offline de citas.  
- **Conectividad:** Acceso a internet para sincronización con servidor.  
- **Sensores opcionales:** GPS para ubicar clínicas cercanas.  

---

## 5. Conclusión

**Stack recomendado:**  
- **Framework:** React Native con Expo  
- **Lenguaje:** TypeScript  
- **IDE:** VS Code con plugins especializados  
- **Hardware:** Cámara, notificaciones push, almacenamiento local  

**Argumentación técnica:**  
React Native ofrece equilibrio entre rendimiento, facilidad de aprendizaje y comunidad. Expo acelera el desarrollo multiplataforma y simplifica la configuración. TypeScript aporta robustez y escalabilidad al código.  

---
