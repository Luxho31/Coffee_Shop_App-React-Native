
# Coffee_Shop_App

Este proyecto es una aplicación móvil desarrollada con React Native. Este README detalla los pasos necesarios para configurar y ejecutar la aplicación en un entorno de desarrollo local.

## Requisitos Previos

- Node.js y npm instalados
- Android Studio instalado y configurado
- Un dispositivo Android o un emulador de Android configurado

## Instalación de Node.js y npm

1. Descarga e instala Node.js desde [nodejs.org](https://nodejs.org/).
2. Verifica la instalación ejecutando:
   ```bash
   node -v
   npm -v
   ```

## Instalación de Android Studio

1. Descarga e instala Android Studio desde [developer.android.com/studio](https://developer.android.com/studio).
2. Durante la instalación, asegúrate de que las siguientes opciones estén seleccionadas:
   - Android SDK
   - Android SDK Platform
   - Android Virtual Device

3. Configura las variables de entorno necesarias:

   - **ANDROID_HOME**: Debe apuntar al directorio donde está instalado el SDK de Android. Por ejemplo:
     ```bash
     C:\Users\<tu_usuario>\AppData\Local\Android\Sdk
     ```

   - Añade las siguientes rutas a la variable de entorno `PATH`:
     ```bash
     %ANDROID_HOME%\platform-tools
     %ANDROID_HOME%\tools
     ```

## Crear un Nuevo Proyecto React Native

1. Navega a la carpeta donde deseas crear tu proyecto y ejecuta:
   ```bash
   npx react-native init Coffee_Shop_App
   cd Coffee_Shop_App
   ```

## Preparar el Proyecto

1. Mueve el proyecto fuera de cualquier carpeta sincronizada con OneDrive para evitar problemas de permisos. Por ejemplo, mueve el proyecto a `C:\Projects\Coffee_Shop_App`.

2. Navega al nuevo directorio del proyecto:
   ```bash
   cd C:\Projects\Coffee_Shop_App
   ```

3. Limpia el caché de Gradle:
   ```bash
   cd android
   ./gradlew clean
   cd ..
   ```

## Iniciar el Servidor de Desarrollo

1. En una terminal, navega al directorio raíz del proyecto y ejecuta:
   ```bash
   npm run start
   ```

## Ejecutar la Aplicación en un Emulador o Dispositivo Android

1. Asegúrate de que el emulador de Android esté en ejecución o que tu dispositivo Android esté conectado y reconocido por `adb`:
   ```bash
   adb devices
   ```

2. En otra terminal, ejecuta:
   ```bash
   npx react-native run-android
   ```

## Solución de Problemas

- Si encuentras problemas durante la compilación, asegúrate de que todas las herramientas estén correctamente instaladas y configuradas.
- Si el problema persiste, proporciona detalles específicos del error para obtener ayuda adicional.

## Enlaces Útiles

- [Documentación de React Native](https://reactnative.dev/docs/getting-started)
- [Documentación de Android Studio](https://developer.android.com/studio)
- [Solución de Problemas de Gradle](https://gradle.org/help/)

---

Este README proporciona una guía paso a paso para configurar y ejecutar tu proyecto React Native en un entorno de desarrollo local. Asegúrate de seguir cada paso cuidadosamente y de verificar que todas las configuraciones estén correctamente establecidas.
