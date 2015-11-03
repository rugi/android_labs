# Instalación de Ceylon en una Mac OS X

## Paso 1. Brew Update
   La manera mas sencilla para instalar Ceylon en una Mac es usando brew.
   Primero actualizamos:

   %> brew update

## Paso 2. Brew Install
   Una vez actualizado, instalamos Ceylon.

   %> brew install ceylon

	==> Downloading http://ceylon-lang.org/download/dist/1_2_0
	==> Downloading from http://downloads.ceylon-lang.org/cli/ceylon-1.2.0.zip
	######################################################################## 100.0%
 	/usr/local/Cellar/ceylon/1.2.0: 661 files, 28M, built in 86 seconds

En caso de que ya lo tuvieras instalado:

  %> brew upgrade ceylon

## Paso 3. Validar instalación.

Para validar la instalación, solo requerimos invocar al compilador con la bandera --version

  %> ceylon --version

	ceylon version 1.2.0 (A Series Of Unlikely Explanations)


La versiòn 1.2.0 de Ceylon está lista para ser utilizada.

-------
Tomado de:
http://ceylon-lang.org/download/

