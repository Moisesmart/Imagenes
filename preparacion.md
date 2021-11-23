# Conexión con Clouding.io

## Preparación del servidor

#### 1- Identificar nuestras credenciales: IP del servidor y la contraseña

#### Una vez que sepamos nuestra IP y contraseña, lo que haremos será conectarnos mediante ssh, para ello necesitarás tener instalado el paquete openssh-server y ssh

![ssh](https://user-images.githubusercontent.com/72433702/143016893-cece6e90-0565-4641-9da4-01beb8ed6635.JPG)

#### 2- Conectarnos al servidor remoto
#### ssh root@IP
#### Nos pedirá confirmación de la conexión por lo que escribiremos la palabra yes
#### Luego tendremos que introducir la contraseña y ya estaremos conectados a nuestro servidor
#### ![Captura1](https://user-images.githubusercontent.com/72433702/143017253-90d31b1b-a066-4ec3-8c2d-298d2a3b304f.JPG)

#### Lo siguiente que haremos será desconectarnos del servidor y en nuestro cliente, meternos en la carpeta ./ssh y ejecutar el comando ssh-keygen

#### Se generarán dos ips, una pública y otra privada, la privada la guardaremos nosotros, la que nos interesa que conozca el servidor es la ip pública por lo que ejecutaremos el siguiente comando:

### ssh-copy-id -i /root/.ssh/id_rsa.pub root@80.240.127.224

#### Tras esto el servidor tendrá nuestras credenciales y podremos conectarnos sin introducir la contraseña
