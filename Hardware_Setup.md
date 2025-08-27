# Hardware Setup

Pasos para preparar el hardware para el entrenamiento de una red neuronal ConvNeXt+ViT

## Instalar Drivers NVIDIA
Identifica qué dispositivo GPU tines y realiza lo siguiente:

1. Descarga de: https://www.nvidia.com/Download/index.aspx
2. Selecciona:
   - Product Type: Selecciona el tipo de producto de tu GPU
   - Product Series: Selecciona la serie de tu GPU
   - Product: Selecciona el modelo de tu GPU
   - Selecciona el sistema operativo que utilizas
3. Descarga e instala

## Instalación y Configuración de Anaconda
Se recomienda instalar Anaconda para crear ambientes aislados del sistema principal

1. Entra a https://www.anaconda.com/download/success
2. Descarga la versión de anaconda dependiendo de tu sistema operativo
3. Instala y ejecuta Anaconda
4. Clic en "Environments"
5. En la parte inferior da clic en "Create"
6. Dale nombre a tu "Enviroironment" por ejemplo, "Skin"
7. Selecciona la versión 3.9.23 de Python
8. Clic en "Create"

## Verificación de instalación de drivers
Para verificar la instalación de los drivers de la GPU, realiza lo siguiente:
1. Da clic en el simbolo de play (triangulo blanco con fondo verde)
2. Clic en "Open Terminal"
3. Teclea lo siguiente: ```nvidia-smi```

Deberías ver información de tu GPU y versión del driver





