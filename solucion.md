
# DOCUMENTACIÓN DE COMO INSERTAR DATOS EN UNA TABLA 
<details>
  <summary>Secciones</summary>
 
  1. [Crear la tabla](#crear-la-tabla)
  2. [Insertando datos en una tabla](#insertando-datos-en-una-tabla)
  3. [Consultar datos](#consultar-datos)
</details>


## Crear la tabla

```sql
-- Selección de SCHEMA
USE sm_data_user;

-- Creación de la tabla 'datos_generales'
CREATE TABLE sm_data_user.datos_generales (
    id INT AUTO_INCREMENT PRIMARY KEY,
    descripcion VARCHAR(255) NOT NULL,
    fecha_registro DATETIME DEFAULT CURRENT_TIMESTAMP
);
```

## Insertando datos en una tabla

```sql
-- Selección de SCHEMA
USE p_siap;
-- Tabla donde se inserntará los datos
INSERT INTO p_siap.datos_sm_v1 (descripcion, fecha_registro) VALUES
('sanmopa2000@gmail.com', NOW()),
('Dirección: Manta, Manabí', NOW()),
```

## Consultar datos

```sql
-- Consulta de todos los datos en la tabla 'datos_generales'
SELECT * FROM sm_data_user.datos_generales;
```




