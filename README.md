# TERMINAL.__GB__
```bash
/ - etc
  - dev
  - home {
          jono {
                work
                photos
                }
          mako
          cory 
         }
  - usr  {
          lib
          }
  - var
```
# comandos
```bash
ls //? muestra las carpetas de donde estamos ubicados
ls -l //? muestra los archivos 
ls -lh //? le da una lectura mas humana
ls -la //? muestra todos los archivos incluido los archivos ocultos
ls -lS //? muestra y ordena por tamanios
ls -lr //? muestra los archivos de la z a la a re reverse
cd //? cd sin parametros te lleva a home
cd nombredelarchivoocarpeta//?entra a el archivo o carpeta
cd .. //? de lleva una carpeta mas atras
clear //? borra la vista dela terminal
pwd //? muestra la ruta de donde estamos
file //? da mucha informacion
mkdir dir1 dir2 etc//? crea un directorio
touch file1 file2 //? crea un archivo
cp filenametocopy newfilenametoname //? copia el archivo
mv filenametomove ..(rutatomove) //? nos permite mover un archivo
mv filename newfilename //? renombra el archivo
rm filename //? remueve el archivo
rm -i filename //? interactivo
rm -rf //? fuerza remover cualquier archivo
rm -ri dir1 //? va a borrar de a un archivo hasta el dir1 preguntandote
rm -r dirname dirmane dirname //? remueve los directorios
head nombredelfile //? muestra el contenido del archivo primeras 10 lineas
head nombredelfile -n 15//? modifica las primeras lineas que tira por defecto ahora son 15
tail nombredelarchivo //? nos muestra las ultimas lineas de un archivo
tail nombredelfile -n 15 //? las ultimas 15 lineas
less nombredelarchivo //? te muestra todo el archivo {
                                                      /nombredelabusqueda //?permitebuscar una palabra
                                                      q //?para salir
                                                      }
xdg-open nombredelarchivo //? te abre el archivo con el editor de texto predeterminado
nautilus nombredelarchivo //? abre el archivo con otra iunterfas grafica
help cd(alguncomando) //?nos muestra todo lo que podemos hacer con ese comando
man cd(alguncomando) //? nos muestra todo lo que podemos hacer con ese comando
info cd(alguncomando) //? nos muestra todo lo que podemos hacer con ese comando
whatis cd(alguncomando) //? nos muestra  que podemos hacer con ese comando


```
# 4 types of comandos 
```bash
type nombredelcomando //? nos muestra el typo de ese comando
```
Un programa ejecutable
```bash

```
Un comando de utilidad de la shell
```bash

```
Una funcion de shell
```bash

```
Un alias
```bash
alias l="ls -lh" //? crea un nuevo comando que remplasa lo que hacia ls -lh
```
