# Diagrama de Flujo del Procedimiento de Solicitud y Evaluación de Etiqueta y Producto Alimenticio en Línea

```mermaid
graph TD;
A[Recabar la Información] -->|Cliente/Usuario| B[Solicitud de Información]
B --> C[Entrega de Requisitos]
C -->|Personal de Ventanilla Única| D[Explicación de Requisitos y Guías]
D --> E[Formas de Presentación de Solicitudes]
E -->|Trámite en Línea o en Oficina| F[Recepción de Datos del Producto y Pago por Servicio]

F -->|Cliente/Usuario| G[Llenado y Envío de Formularios en Línea]
G -->|Plataforma Virtual| H[Adjuntar Imágenes y Documentos]
H --> I[Verificación de Información]
I --> J[Pago por Servicio Solicitado]
J -->|Verificación de Pago| K[Evaluación y Emisión del Documento]
K -->|Encargado de Evaluación| L[Evaluación de Etiquetas]
L --> M[Verificación de Información y Documentación]
M --> N[Dictamen de Etiquetas]

N -->|Encargado de Evaluación| O[Aprobación]
N -->|Encargado de Evaluación| P[Observación]

O --> Q[Emisión del Certificado]
Q -->|Profesional Designado con Firma Digital| R[Registro e Impresión del Certificado]
R --> S[Recepción del Certificado Digital]

P -->|Cliente/Usuario| T[Corrección de la Solicitud]
T --> L

S --> U[Archivo del Documento Digital]
U -->|Área de Sistemas| V[Almacenamiento en Base de Datos]
S --> W[Archivo por Parte del Usuario]
W -->|Cliente/Usuario| X[Archivado de Documentos Físicos]

subgraph Solicitud y Evaluación
  A --> F
end

subgraph Emisión del Documento
  K --> S
end

subgraph Archivo del Documento
  U --> X
end
