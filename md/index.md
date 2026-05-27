# Sistema DNS

![Introducción DNS](images/dns-intro.png)

## Introducción

El sistema **DNS (Domain Name System)** es una de las tecnologías fundamentales de Internet.

Su función principal consiste en traducir nombres de dominio fáciles de recordar en direcciones IP utilizadas por los equipos para comunicarse.

???- example "Por ejemplo:"

    ```text
    www.google.com
    ```

    Se transforma en:

    ```text
    142.250.184.196
    ```

---

## ¿Por qué es necesario?

Sin el DNS tendríamos que memorizar direcciones IP numéricas para acceder a cualquier página web o servicio.

Gracias al DNS:

- Navegar es mucho más sencillo.
- Los dominios están organizados jerárquicamente.
- Internet puede crecer de forma escalable.
- Los servicios son más fáciles de administrar.

---

## Funcionamiento básico

Cuando un usuario introduce una dirección web:

1. El navegador consulta la caché local.
2. El sistema operativo revisa su caché DNS.
3. Se consulta un servidor DNS.
4. El servidor localiza la IP correspondiente.
5. El navegador conecta con el servidor web.

---

## Estructura de un dominio

Ejemplo:

```mermaid
graph TD

A["www.ejemplo.com"]

A --> B["www"]
A --> C["ejemplo"]
A --> D[".com"]

B --> E["Subdominio"]
C --> F["Dominio principal"]
D --> G["TLD<br>(Top Level Domain)"]

G --> H["Dominio de nivel superior"]
```

---

!!! tip "Importancia del DNS"

    El DNS es imprescindible para el funcionamiento de Internet moderno y permite que millones de servicios puedan localizarse de manera rápida y eficiente.
