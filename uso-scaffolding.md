# Uso de scaffolding

Para poder usar scaffolding desde la cli de `dotnet` se debe instalar la herramienta `dotnet-aspnet-codegenerator`.  
Esto lo podemos hacer desde una shell (powershell, bash, etc) y ejecutando el siguiente comando:  

```powershell
dotnet tool install -g dotnet-aspnet-codegenerator
```

## Scaffolding de controllers

Una vez instalada la herramienta ya podemos proceder a la creación de los scaffolding, en particular a la creación de scaffolding de controladores mvc usando entity framework y generando vistas asociadas.  
Para crear el scaffolding de un controller mvc con actions y views usando entity framework podemos hacerlo a través de este comando:  

```powershell
dotnet aspnet-codegenerator controller -m MODELO_CON_NAMESPACE -dc DB_CONTEXT_NAMESPACE -name NOMBRE_DEL_CONTROLADOR -outDir Controllers -async -scripts -udl -f
```

Un ejemplo del uso con modelos, dbcontext y nombre de controller:  

```powershell
dotnet aspnet-codegenerator controller -m mi_namespace.Models.Alumnos -dc mi_namespace.Database.InstitutoDbContext -name AlumnosController -outDir Controllers -async -scripts -udl -f
```

[Volver](README.md)
