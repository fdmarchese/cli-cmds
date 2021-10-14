# Creación de proyectos

Para crear nuevos proyectos desde la cli de `dotnet` lo primero que se debe hacer es posicionarse en la carpeta donde se quiere crear el proyecto. 
Una vez posicionado donde corresponse utilizando una shell (powershell, bash, etc) procedemos a la creación del proyecto: 

## Nuevo proyecto MVC netcore 3.1

```powershell
dotnet new mvc -au None --framework netcoreapp3.1 --no-https
```

## Nuevo proyecto consola netcore 3.1

```powershell
dotnet new console --framework netcoreapp3.1
```

[Volver](README.md)