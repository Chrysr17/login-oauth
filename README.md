# Login Básico con Google OAuth2 - Spring Boot

Demo de login simple con Google OAuth2 en Spring Boot (puerto 8040).

## Configuración

1. Obtener credenciales en [Google Cloud Console](https://console.cloud.google.com/).  
   URI de redirección: `http://localhost:8040/login/oauth2/code/google`

2. Cambiar `application.properties`:
spring.security.oauth2.client.registration.google.client-id=${GOOGLE_CLIENT_ID}
spring.security.oauth2.client.registration.google.client-secret=${GOOGLE_CLIENT_SECRET}
spring.security.oauth2.client.registration.google.scope=profile,email
