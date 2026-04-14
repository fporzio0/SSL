# Variable por si quiero cambiar de versión de C en algun momento
CFLAGS=-std=c23 -Wall
NOMBREDELBINARIO = hello

# Regla para compilar
build: hello.c 
	gcc hello.c -o $(NOMBREDELBINARIO) $(CFLAGS)

# Regla para ejecutar
# Al escribir "run: build" le estoy diciendo al make "Para ejecutar run, primero asegurate de que la regla build se haya cumplido con éxito". 
# Ademas, si pasamos como parametro "hello.exe" quedamos atados a Windows, ya que esa extension es propia del mismo. Si quisieramos migrar el 
# codigo a Linux, daría error
run: build
	./$(NOMBREDELBINARIO)