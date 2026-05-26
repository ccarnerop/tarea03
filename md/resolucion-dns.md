# Resolución DNS



La resolución DNS es el proceso mediante el cual un nombre de dominio se convierte en una dirección IP.

---

## Proceso de resolución

Cuando un usuario escribe una URL en el navegador se producen los siguientes pasos:

1. Consulta de caché local.
2. Consulta del sistema operativo.
3. Consulta al DNS recursivo.
4. Consulta a servidores raíz.
5. Consulta al servidor TLD.
6. Consulta al servidor autoritativo.
7. Respuesta con la dirección IP final.

![Proceso de resolución DNS](images/dns-resolucion1.png)

---

## Esquema simplificado

```text
Cliente
   ↓
DNS Recursivo
   ↓
Servidor Root
   ↓
Servidor TLD
   ↓
Servidor Autoritativo
```

---

## Caché DNS

Las respuestas DNS se almacenan temporalmente para acelerar futuras consultas.

Ventajas:

- Menor tiempo de respuesta.
- Menor tráfico de red.
- Mejor rendimiento.

---

## TTL

El TTL (Time To Live) indica cuánto tiempo permanece almacenada una respuesta DNS en caché.

---

## Ejemplo real

```text
www.wikipedia.org
```

Resolución:

```text
www.wikipedia.org → 208.80.154.224
```