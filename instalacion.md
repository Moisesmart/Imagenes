## INSTALACIÓN k0s

## INSTALACIÓN PARA 2 SERVIDORES Ó PARA UN SÓLO SERVIDOR
### -----------------
### 2 SERVIDORES
### -----------------

### Uso de 2 servidores ( controller + worker )

#### Una vez que tenemos preparada la conectividad con las máquinas procedemos a descargar k0s, yo he utilizado wget para descargarme el paquete k0sctl directamente y el comando es el siguiente:

wget https://github.com/k0sproject/k0sctl/releases/download/v0.8.4/k0sctl-linux-x64 && mv k0sctl-linux-x64 k0sctl && chmod 777 k0sctl

#### COMPROBAMOS QUE TENEMOS K0SCTL INSTALADO

## Ejecutamos ./k0sctl

#### Desde el usuario que es desde donde hemos descargado el paquete k0sctl

### EJECUTAMOS ./K0SCTL INIT
#### Al ejecutar ./k0sctl init lo pasaremos a un fichero yaml con el comando >

## Editamos e fichero yaml recientemente creado, modificamos el address y el role

## En address colocaremos la IP de nuestro servidor y en role podemos asignarle tanto control-plane como worker, yo le he asignado el rol como controller+worker
![Captura de pantalla de 2021-11-24 17-41-00](https://user-images.githubusercontent.com/72433702/143285279-dba51421-ed67-4d78-9639-e531f26d445d.png)



#### Tras configurar el fichero yaml ejecutaremos un apply con la siguiente orden:

## ./k0sctl apply --config k0sctl.yaml


### Este es el resultado:
![Captura de pantalla de 2021-11-24 17-39-54](https://user-images.githubusercontent.com/72433702/143283425-65116edd-4474-42e6-87c3-7cded792f739.png)



### ---------------------
### 1 SERVIDOR
### ---------------------

### 2 Pasos: Descarga e intalación  
#### 1. Descarga con curl
![Captura de pantalla de 2021-11-26 10-26-04](https://user-images.githubusercontent.com/72433702/144210154-a782b709-4d2f-4775-bba1-158211716206.png)

#### 2. Instalar
![Captura de pantalla de 2021-12-01 08-31-29](https://user-images.githubusercontent.com/72433702/144210197-b86bbec5-3a26-4cf0-a23f-fef9105d5d96.png)

#### 3. Detalles de k0s
![Captura de pantalla de 2021-12-01 08-33-31](https://user-images.githubusercontent.com/72433702/144210214-f1ad0223-673c-45cb-a268-f7c62c3f89a7.png)

#### 4.Comprobación de la instalación

![k0s1](https://user-images.githubusercontent.com/72433702/145805799-61e1b6f0-2fb6-41b0-bd14-bbc411549fc7.JPG)
![k0s2](https://user-images.githubusercontent.com/72433702/145805821-4f4a915f-094c-46e3-8290-4900d858dcf8.JPG)
![k0s3](https://user-images.githubusercontent.com/72433702/145805840-5b6255ef-3a07-4b75-b47f-92faf0a3edbc.JPG)
![k0s4](https://user-images.githubusercontent.com/72433702/145805858-10769ab8-386b-4ae9-a987-d9fe46838af1.JPG)
![k0s5](https://user-images.githubusercontent.com/72433702/145805862-a0145669-59a7-41f5-8cf2-97703749247d.JPG)

