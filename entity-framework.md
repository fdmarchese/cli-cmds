# Entity framework

El manejo de migraciones y actualización de la base de datos utilizando entity framework puede ser gestionado a través del uso de la cli de `dotnet`. 

## Instalación 

Lo primero que debemos hacer es instalar el componente si es que no lo tenemos instalado. 

Utilizando cualquier shell (powershell, bash, etc) en cualquier directorio ejecutamos el siguiente comando: 

```powershell
dotnet tool install -g dotnet-ef
```

## Agregando migraciones

Una vez instalado el componente podemos proceder a la creación de migraciones. 
Dentro del shell elegido nos posicionamos en la carpeta del proyecto sobre el cual queremos agregar las migraciones y luego ejecutamos el siguiente comando reemplazando `NOMBRE_DE_LA_MIGRACION` con el nombre que le queremos dar a nuestra migración: 

```powershell
dotnet ef migrations add NOMBRE_DE_LA_MIGRACION
```

## Actualizando/Creando la base de datos

Cuando nuestro proyecto ya cuenta con migraciones que contienen las instrucciones específicas para crear y actualizar nuestra base de datos podemos proceder a la ejecución del comando de actualización de la base de datos (recordar que la base de datos destino es la que tenemos configurada en nuestro código, generalmente en el `Startup.cs`): 

```powershell
dotnet ef database update
```

[Volver](README.md)