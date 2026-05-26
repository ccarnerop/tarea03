# ¿Qué es el DNS?



El **Domain Name System** es un sistema distribuido y jerárquico encargado de relacionar nombres de dominio con direcciones IP.

---

## Componentes principales
![Componentes DNS](images/dns-componentes.png)

### Dominio

Nombre fácil de recordar que identifica un servicio en Internet.

Ejemplo:

```text
openai.com
```

---

### Dirección IP

Identificador numérico único de un dispositivo dentro de una red.

Ejemplo IPv4:

```text
192.168.1.100
```

Ejemplo IPv6:

```text
2001:db8::1
```

---

### Servidor DNS

Equipo encargado de responder consultas DNS.

Existen varios tipos:

- Servidores raíz
- Servidores TLD
- Servidores autoritativos
- Servidores recursivos

---

## Jerarquía DNS

```text
.
├── .com
├── .org
├── .net
└── .es
```

Cada dominio puede contener subdominios adicionales.

---

## Resolución directa

Transforma un dominio en una dirección IP.

```text
google.com → 142.250.184.196
```

---

## Resolución inversa

Transforma una dirección IP en un nombre de dominio.

```text
142.250.184.196 → google.com
```

---

## Ventajas del DNS

- Facilita la navegación.
- Permite escalabilidad.
- Mejora la organización de Internet.
- Permite redundancia y tolerancia a fallos.