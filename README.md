# TERMINAL.__GB__

*sistema de archivos de linux*
```bash
/`raiz`     - etc
            - dev
            - home`~ simbolo que representa al home en bash`
                   {
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
# visual studio
```bash
code .nombredelarchivo //? abre el archivo en visual
```
# comandos
```bash
`borrar gabriel nestor brufau borrar gabriel nestor brufau borrar`
ls ` muestra las carpetas de donde estamos ubicados`
ls -l ` muestra los archivos `
ls -lh ` le da una lectura mas humana`
ls -la //? muestra todos los archivos incluido los archivos ocultos
ls -lS //? muestra y ordena por tamanios
ls -lr //? muestra los archivos de la z a la a re reverse
ls *.txt //? busca todos los archivos que terminan en txt
ls primeraspalabrasdelarchivo* `busca todos los archivos
   que conincidan con las palabras que pongas antes del *`
ls primerasletrasdelarchivo? //? busca todas las coincidencias que tengan las letras y solo un caracter final
ls primerasletrasdelarchivo??? //? busca todas las coincidencias que tengan las letras y solo tres caracter final
ls [[:upper:]]* //? busca todas las carpetas que empiezan con uppercat mayusculas
ls -d [[:upper:]]* //? busca todas los directorios que empiezan con uppercat mayusculas
ls [[:lower:]]* //? busca todas las carpetas que empiezan con minusculas
ls nombrefile > nombrefile //? copia/sobrescribe lo que hay en el primero al segundo
ls nombrefile >> nombrefile //? concatena los archivos con el nuevo nombre que le des si no existe lo crea
ls archivoquedaunerror 2> error.txt //? crea un archivo que dentro podemos visualizar el errror con el comando head
ls archivoquenosavemoscomoresultara > output.txt 2>&1 //? si no sabemos si el archivo nos va a arrojar un arror o reject
ln -s rutade/ejemplo linkdeejemplo //? acceso directo

less nombredelarchivo` te muestra todo el archivo de manera
interactiva 
{
 "/nombredelabusqueda" : permitebuscar una palabra
 "q" : para salir
 `
}
                                                      }`
cd ` cd sin parametros te lleva a home`
cd nombredelarchivoocarpeta `entra a el archivo o carpeta`
cd .. ` de lleva una carpeta mas atras`

clear //? borra la vista dela terminal

pwd ` muestra la ruta de donde estamos`

file ` da mucha informacion`
file nombredelarchivo `da mucha informacion del archivo`
file ./path/archivo.arch `lo mismo pero para cuando estamos fuera`

find ./ <name nombredelarchivo //? busca todos los archivos que se llamen asi
find ./ -name *.txt | less //? busca todos los archivos que terminen en eso y te da info
find ./ -type f -name nombredelfile //? busca por type
find ./ -type d -name nombredeldirectorio
find ./ -type f -name *.log //? busca el archivo .log
find ./ -size 20M //? busca los archivos por taman:o mayores a 20 megas
mkdir dir1 dir2 etc//? crea un directorio
man comando //? man recive como parametro un comando a consultar es como un manual de uso
touch file1 file2 //? crea un archivo
> nombredelarchivo.txt //? crea un archivo de texto
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
tail -f //? queda ala escucha  de algun cambio en el archivo

xdg-open nombredelarchivo `te abre el archivo con el editor de
texto predeterminado`
nautilus nombredelarchivo `abre el archivo con otra iunterfas
grafica`
nombredelprograma archivo `abrira el archivo?`
help cd(alguncomando) //?nos muestra todo lo que podemos hacer con ese comando
man cd(alguncomando) //? nos muestra todo lo que podemos hacer con ese comando
info cd(alguncomando) //? nos muestra todo lo que podemos hacer con ese comando
whatis cd(alguncomando) //? nos muestra  que podemos hacer con ese comando
echo "hola mundo" //? solo genera una salida en la terminal
echo $nombredelavariabledeentorno //? imprime la variable de entorno
cat unarchivo segundoarchivo //? concatena archivos
cat nombredelarchivo //? lee el archivo
cat /etc/lsb-release //? aca vemos que distribucion de ubuntu toca
cat > nombredelarchivo //? permite escribir dentro del archivo Ctrl d para dejar de escribir
chmod numerosenmodooctal nombredelarchivo //? cambia los permisos del archivo
chmod u-r nombredelarchivo //? la u es de usuario el menos de de quitar la r es de lectura
chmod u+r nombredelarchivo //? le da los permisos de lectura
chmod u-x,go=w nombredelarchivo //? esto le da al usuario un permiso de ejecucion,go, al grupo como a otros le da un permiso de write
whoami //? le pregunta ala maquina quienes somos
which nombredelprograma //? busca la ubicacion del programa
id //? nos da informacion del usuario extra
su nombredeusuario //? cambiamos de usuario
su root //? nos cambiamos al mitico user root 
sudo //? te da los permisos del user root podras borrar archivos root desde cualquier user
passwd //? nos permite cambiar la contrasenia de cualquier user
grep //? es un comando que permite filtrar alguna palabra que busques en determinado archivo
```
# tipos de archivos
```bash
- //?un archivo normal
d //?un directirio
l //? un link simbolico
b //?un archivo de bloque especial son los archivos que manejan la informacion de los bloques de datos como una USB
```
# tipos de modo
```bash
duen:o  rwx 111
grupo  r-x  101
word  r-x  101
```
# modo octal
```bash
octal   binario   permisos
0       000       ---
1       001       --x
2       010       -w-
3       011       -wx
4       100       r--
5       101       r-x
6       110       rw-
7       111       rwx
```
# tipos de permisos
```bash
r //? permisos de lectura
x //? permisos de ejecucion
w //? permisos de escritura
a //? todos
g //? grupos
u //? usuarios
son nueve caracteres
rrrxxxwww //? los tres primeros son para el usuario los tres siguientes son para el grupo y los ultimos tres son para otros usuarios
chmod u+x algunarchivo.txt //? le da los permisos al usuario de x ejecucion
chmod +x archivo.txt //? le da los permisos de ejecucion a todos 
formato octal
r = 4
w = 2
x = 1
rwx-xr--x = 751
sudo chown rood:rood archivo.txt //? cambia el propietario del archivo 

```
# modo simbolico
```bash
simbolo       significado
u             solo para usuarios
g             solo para el grupo
o             solo para otros(es el word)
a             Aplica para todos
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
## funciones con comandos
```bash
ls; mkdir holi; cal //? el punto y coma nnos permite correr multiples comandos
ls & date & cal //? permite ejecutar varios comandos de forma asincrona
mkdir test && cd test //? crea la carpeta test y si la crea entra a esta
cd archivoquenoexiste || touch archivo.txt && echo "si funca"//? no le importa si algun procesi falla continua con el otro
```
# modificar los permisos en la terminal
```bash
chmod 755 nombredelarchivo //? cambia los permisos del archivo

```
# variables de entornos
```bash
printenv //? nos muestra todas las varialbles de entornos que tenemos configuradas
//para modificar las variablkes de entorno
ls -la buscamos bashrc //? miramos como si se encuentra ese erchivo
code .bashrc //? lo abrimos con visual estudio

```
# utilidades de red
```bash
ifconfig //? muestra enformacion de red direcciones puertos sertvidores
ping www.google.com //? da informacion de la conectividad de una pagina
curl www.google.com //? trae el codigo de la pagina
curl www.google.com //? > index.html
wget www.google.com //? descarga el archivo a la computadora
traceroute www.google.com//? todas las computadoras que intervienen que intervienen en el camino para llegar a google
netstat -i //? muestra los dispocitivos de red

```
# comprimiendo archivos 
```bash
tar -cvf archivoacomprimir.tar nombredeldirectorio //? tar comprime archivos -c (comprimir) v(muestra el ouput en la terminal) f (porque va a comprimir un file)
tar -cvzf archivoacomprimir.tar.gz nombredeldirectorio //? tar comprime archivos -c (comprimir) v(muestra el ouput en la terminal) f (porque va a comprimir un file) z (le comprime en archivo.zip)
tar -xzvf archivoadescomprimir.tar.gz
zip -r archivoacomprimir.zip nombredeldirectorio //? comprime el archivo en zip
unzip archivoadescomprimir.zip 
```
# manejo de procesos
```bash
ps //? muestra los procesos que estan corriendo en nuestra terminal actualmente
ps -fy //? ft listado de las consolas
ps aux //? nos muestra el usuario, el numero del proceso, cuanta cpu, cuanta memoria , que tty estoy utilizando y cualcomando esta realizando este proceso
ps aux | grep nombredeluser //? nos muestra los prosesos ejcutados por el usuario

top //? muestra los procesos que estan usando mas recursos
kill //? mata procesos desde nuestra terminal
kill -9 numero del proceso o PID //? esto mata el proceso -9 para que no te pregunte nada mas
```
# vim
```bash
vim //? para entrar a vim
:q //? para salir de vim
vim index.html //? crea un archivo index en el aditor
```
# Terminal
```bash
ssh localhost //? nos crea una nueva coneccion en el sistema operativo 
tty //? para ver la terminal en la que estoy conectado
w //? para ver que usuarios estan corriendo en la terminal
who //? una informacion mas sutil de los usuarios conectados
chvt //? crea una terminal creo?
jobs //? muestra los procesos parados
fg //? te trae de nuevo el proceso parado ejemplo en vim
```
# servidores
```bash
nohup ./nombredelarchivo.ejm //? esto nos da un archivo nohup.out de lo que hizo el proceso muy util en los despliegues de servidores
top //? nos muestra los procesos de nuestro equipo
cat /proc/cpuinfo | grep "processor" //? nos da los procesadores que tenemos
sudo ps auxf | sort -nr -k 3 | head -5 //? nos muestra los 5 procesos que estan consumiendo mas cpu
sort //? ordena 
head //? te da una vista de ayuda
sudo ps auxf | sort -nr -k 4 | head -5 //? nos muestra el cunsumo de la memoria ram
free //? nos da la memoria ram
free -h //? nos da la memoria ram dada en gib o megabyte
du //? nos da los datos del disco?
htop //? podemos organizar mejor los procesos para entender mejor

```
# parametros de red
```bash
ifconfig //? nos da algunos datos como ip
ip a //? tambien muestra la informacion de la red
hostname //? nos da el nombre como identificamos este equipo en cadda una de la redes
route -n //? nos da la puerta predeterminada a nuestra red
nslookup google.com //? nos muestra la direccion de ese dominio
curl //? descarga siertas cosas del sistema operativo curl puede realizar simulaciones como lo hace un sofware como posman pero desde  la consola
curl localhost //? esto interactua como posman
wget algundominio //? esto trae informacion de el dominio
```
# Manejo de paquetes
```bash
Debian/ubuntu
.deb
dpkg-reconfigure
repositorios apt
/var/lib/dpkg //? aca se localiza la base de datos DPKG
dpkg -l //? lista todos los debs instalados en la maquina
dpkg -i paquete.deb //? realiza la instalacion de un paquete
apt install paquete
dpkg -r paquete.deb //? remover un paquete del sistema
dpkg-reconfigure paquete //? volver a ejecutar el asistente de configuracion si esta disponible por ejemplo ajustar la hora del servidor
apt-get update //? actualizamos los indices del paquete apt va a pedir sudo
sudo apt-get update
sudo apt-get upgrade //? una vez actualizados los indices este comando descarga 
sudo apt dist-upgrade //? es un poco mas desprolijo te actualiza los paquetes pero tendras que reiniciar la maquina
sudo anap install canonicallivepatch //? permite instalar paquetes con dist-update sin tener que reiniciar
sudo apt search newpaquete //? busca un paquete en especifico
dpkg -l //? lista los paquetes que tenemos en nuestro sistema operativo
sudo dpkg-reconfigure tzdata //? esto reconfigurara la hora a la que elijamos
sudo dpkkg-reconfigure nombredelpaquete
snap //? es una version mas nueva de apt que es mas replicable en otras distribuciones linux
sudo snap search aws-cli //? nos muestra no se bien que
sudo snap refresh --list //? nos muestra los paquetes a actualizar
sudo snap info aws-cli //? nos muestra info del paquete



```
# monitoreo de base de datos
```bash
sudo apt install build-essential libgd-dev openssl libssl-dev unzip apache2 php gcc libdbi-perl libdbd-mysql-perl 
```
# descomprimir archivos
```bash
tar //? descomprime y desempaqueta
tar xvzf archivo.tar.gz //? x extraer v para que tenga verbouse (por pantalla mostrara lo que esta realizando) z porque es un formato que esta enpaquetado y comprimido f le indica que va a ir un archivo
```
