# cli-cmds
comandos de cli's útiles


Crear nuevo proyecto mvc con netcore 3.1:

```bash
dotnet new mvc -au None --framework netcoreapp3.1 --no-https
```

## dotnet-ef

Para manejar las migrations y updates utilizando entity framework

```bash
dotnet tool install -g dotnet-ef

## dotnet-aspnet-codegenerator

Instalarlo en la máquina:

```bash
dotnet tool install -g dotnet-aspnet-codegenerator
```


Para hacer scaffolding de un controller mvc con actions y views usando entity framework:

```bash
dotnet aspnet-codegenerator controller -m MODELO_CON_NAMESPACE -dc DB_CONTEXT_NAMESPACE -name NOMBRE_DEL_CONTROLADOR -outDir Controllers -async -scripts -udl -f
```

Ejemplo:

```bash
dotnet aspnet-codegenerator controller -m mi_namespace.Models.Alumnos -dc mi_namespace.Database.InstitutoDbContext -name AlumnosController -outDir Controllers -async -scripts -udl -f
```
