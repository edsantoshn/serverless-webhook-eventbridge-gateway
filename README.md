# serverless-webhook-eventbridge-gateway
🚀 Gateway serverless para webhooks construido con AWS EventBridge, diseñado para manejar alta concurrencia y garantizar la entrega confiable de eventos.

# 🎯 Características
Procesamiento asíncrono de webhooks
Control de concurrencia para evitar sobrecarga
Manejo automático de reintentos
Cola de mensajes fallidos (DLQ)
Validación de payloads
Seguridad mediante API Keys

# 🏗️ Arquitectura
![architecture](imgs/architecture.png?raw=true)
API Gateway para ingesta de webhooks
EventBridge para enrutamiento de eventos
SQS para buffering y control de carga
Lambda para procesamiento asíncrono
DLQ para manejo de errores

# 🛡️ Límites y Protecciones
Control de concurrencia en Lambda
Protección contra picos de tráfico
Manejo del límite soft de AWS Lambda (1000 ejecuciones concurrentes)


# 🔧 Tecnologías
AWS CloudFormation
Amazon API Gateway
Amazon EventBridge
Amazon SQS
AWS Lambda
IAM Roles & Policies