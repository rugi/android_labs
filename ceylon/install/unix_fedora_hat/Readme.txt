La instalación en Fedora-RedHat es vía un RPM.

La pagina de descarga proporciona el rpm:

    http://ceylon-lang.org/download/

Para la fecha de esta instalación de prueba (03/Nov/2015) el rpm descargable es el siguiente:

    ceylon-1.2.0-1.2.0-0.noarch.rpm........14224372

Paso 1. Colocamos el archivo en una carpeta temporal.

    %tmp> ls 
    -rw-r-----. 1 rugi rugi 14224372 Nov  3 22:17 ceylon-1.2.0-1.2.0-0.noarch.rpm

Paso 2. Le damos permisos de ejecución:

    %tmp>chmod +x ceylon-1.2.0-1.2.0-0.noarch.rpm
    %tmp>ls -lrt
    -rwxr-x--x. 1 rugi rugi 14224372 Nov  3 22:17 ceylon-1.2.0-1.2.0-0.noarch.rpm

Paso 3. Instalamos el rpm (toma en cuenta que el uso de _rpm_ requiere permisos de _root_)

    %tmp>sudo rpm -ivh ceylon-1.2.0-1.2.0-0.noarch.rpm
        Preparing...                          ################################# [100%]
        Updating / installing...
           1:ceylon-1.2.0-0:1.2.0-0.fc22      ################################# [100%]

Paso 4. Validamos la instalación.


    %tmp>ceylon --version
        ceylon version 1.2.0 (A Series Of Unlikely Explanations)

La instalación del rpm ha sido completada.    



NOTA:
En el ejemplo, rpm ha sido ejecutado con los parámetros: -ivh.
-----------------------
Tomado de: *man rpm*

    GENERAL OPTIONS
        -v     Print verbose information - normally routine progress messages will be displayed.
  
    INSTALL AND UPGRADE OPTIONS
        {-i|--install}................. This installs a new package.
        OPTION:
            -h, --hash....... Print 50 hash marks as the package archive is unpacked.
-----------------------



