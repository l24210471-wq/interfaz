
### Asistencia de Inteligencia Artificial
 **Nivel de participación de IA**: 3
- **Prompts utilizados**:
  - "Traduce e interpreta la información de las fuentes manteniendo la terminología técnica de ARM64, ARM32 y RISC-V."
  - "Analiza el contenido sobre vectorización y filtra únicamente los datos relevantes para la comparación de arquitecturas."
  - "Depura el código fuente generado en ensamblador y adapta la sintaxis para mantener cohesión en lenguaje Markdown."

- **Herramientas utilizadas**:
  - Gemini
  - DeepSeek
  - ChatGPT


- **Reflexión personal**:
  Con las LLM entendí la convención de llamadas, pero inventó un número de syscall. Esto reforzó mi hábito de validar contra la documentación oficial y con `strace`.
  
### Explicación propia de una decisión técnica central
Para optimizar el procesamiento paralelo utilicé de manera teórica **vectorización con NEON (ARM64/ARM32)** para cargas de trabajo con registros de tamaño fijo de 128 bits, garantizando la compatibilidad con hardware actual como AWS Graviton.

- **Fecha**: 2026-09-21

- **Plataforma utilizada**: Markdown online
