# Tipos de Arquitectura de Sistemas

## 1. Sistema Monolítico
- Todo el sistema está empaquetado como una sola aplicación.
- La interfaz, la lógica de negocio y la base de datos están integradas.
- **Ejemplo:** Aplicaciones antiguas de escritorio o servidores web PHP tradicionales.

---

## 2. Arquitectura de Microservicios
- El sistema está dividido en servicios pequeños, independientes y desplegables de forma separada.
- Cada microservicio tiene su propia lógica y, a veces, su propia base de datos.
- **Ejemplo:** Amazon, Netflix, aplicaciones modernas en la nube.

### Ventajas:
- Escalabilidad independiente.
- Despliegues rápidos y específicos.

### Desventajas:
- Complejidad en la comunicación y monitoreo.

---

## 3. Arquitectura en Capas (N-Tier)
- Separación lógica en capas: presentación, lógica de negocio, acceso a datos.
- Puede estar en un solo servidor o distribuido.
- **Ejemplo:** Aplicaciones Java con frontend, backend y base de datos separados.

### Ventajas:
- Mejor organización y mantenimiento que el monolito.

### Desventajas:
- Sigue siendo más acoplado que los microservicios.

---

## 4. Arquitectura Orientada a Servicios (SOA)
- Antecesora de los microservicios.
- Servicios más grandes que los microservicios, que comparten datos y lógica.
- Utiliza un **Enterprise Service Bus (ESB)** para comunicar servicios.
- **Ejemplo:** Grandes ERP y sistemas bancarios antiguos.

---

## 5. Arquitectura Serverless (Sin Servidor)
- No gestionas servidores directamente.
- Usas funciones pequeñas que se ejecutan en respuesta a eventos.
- **Ejemplo:** AWS Lambda, Azure Functions.

### Ventajas:
- Escala automáticamente.
- Pagas solo por uso.

### Desventajas:
- Limitaciones de tiempo de ejecución y control.

---

## 6. Arquitectura basada en Eventos (Event-Driven)
- Los componentes reaccionan a eventos publicados en colas o brokers (ej: Kafka, RabbitMQ).
- Muy utilizada en sistemas altamente desacoplados y en tiempo real.
- **Ejemplo:** Sistemas de notificaciones, comercio electrónico.

---

## Resumen Visual

| Tipo de Arquitectura      | Características                 | Ejemplos                |
|---------------------------|---------------------------------|-------------------------|
| Monolítica                | Todo junto                      | Apps antiguas           |
| Microservicios            | Módulos pequeños independientes | Netflix, Amazon         |
| En Capas (N-Tier)         | Separación por lógica           | Apps Java tradicionales |
| SOA                       | Servicios grandes integrados    | ERPs antiguos           |
| Serverless                | Basado en funciones y eventos   | AWS Lambda apps         |
| Basada en Eventos         | Comunicación mediante eventos   | Apps en tiempo real     |
