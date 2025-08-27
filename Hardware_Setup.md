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

## Instalación de CUDA Toolkit
Para programar ConvNeXt + ViT necesitamos pytorch y la versión de CUDA compatible para ello es la 11.8:
1. Ve a: https://developer.nvidia.com/cuda-11-8-0-download-archive
2. Selecciona Windows → x86_64 → 11 → exe (local)
3. Descarga e instala

## Instalación de Pytorch con soporte GPU
En la terminal, ejecuta:
```pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118```

## verifica que Pytorch detecte tu GPU
1. En tu terminal escribe ```python```y dale enter
2. Se abrirá la interfaz para programar en python
3. Introduce el siguiente código:

```python
import torch

print(f"PyTorch version: {torch.__version__}")
print(f"CUDA available: {torch.cuda.is_available()}")
print(f"CUDA version: {torch.version.cuda}")
print(f"GPU name: {torch.cuda.get_device_name(0)}")
print(f"GPU memory: {torch.cuda.get_device_properties(0).total_memory / 1024**3:.1f} GB")
```















