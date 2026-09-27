# EducaAndOS-Root
Binario para la escalada de privilegios a `root` en EducaAndOS y EducaAndOS V2.

EducaAndOS y EducaAndOS V2 utilizan versiones del kernel de Linux vulnerables al fallo [copyfail](https://copy.fail/) (CVE-2026-31431). Debido a que algunas dependencias necesarias para compilar y ejecutar el exploit no están presentes por defecto en el sistema, este binario se distribuye precompilado de forma estática con todas las dependencias integradas.

Al ejecutarse, el binario genera una shell interactiva con permisos de superusuario. Si te encuentras en un entorno de escritorio, puedes lanzar `gnome-terminal` desde dicha shell para abrir una ventana gráfica independiente como `root`.

## Modo de uso

1. Descarga el binario **[aquí](https://raw.githubusercontent.com/MiloDev123/EducaAndOS-Root/refs/heads/main/root)**.
2. Abre una terminal y asigna permisos de ejecución:

```bash
chmod +x root
./root
```

3. Se abrirá la shell con privilegios elevados.

<img width="1755" height="209" alt="image" src="https://github.com/user-attachments/assets/405318e9-4652-4c45-ad4a-9e0541b4c0b0" />

> **Aviso de responsabilidad:** Este proyecto ha sido desarrollado exclusivamente como prueba de concepto (PoC) con fines educativos, de investigación y auditoría de seguridad. El autor no se hace responsable del uso indebido que terceros puedan dar a este software. Su ejecución en redes, servidores o equipos institucionales sin la autorización explícita de sus administradores puede constituir una infracción disciplinaria o legal.
