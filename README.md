from dhooks_lite import Webhook
import re
from colorama import Fore


hook = Webhook("INSERTAR KEY DE WEBHOOK")


print(Fore.BLUE + """
 ▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄   ▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄
█─█─█─▄▄─█─▄▄─██─█─▄███─▄▄▄▄█▄─▄▄─█▄─▀█▄─▄█▄─▄▄▀█
█─▄─█─██─█─██─██─▄▀████▄▄▄▄─██─▄█▀██─█▄▀─███─██─█
▀▄█▄█▄▄▄▄█▄▄▄▄██▄█▄▄▀▀▀▄▄▄▄▄█▄▄▄▄▄█▄▄▄██▄▄█▄▄▄▄█▀
""")

name = input(Fore.CYAN + "1. Introduce tu nombre: ")

mensaje = input(Fore.CYAN + "2. Introduce el mensaje: ")

censura = ("http")


if re.search(censura, name) is not None:
    print(Fore.RED + "No puedes colocar links en tu nombre")
    exit()

if re.search(censura, mensaje) is not None:
    print(Fore.RED + "No puedes colocar links en tu mensaje")
    exit()

else:
    hook.execute(name + ' **>>** ' + mensaje)
    print(Fore.BLUE + "Listo! Mensaje enviado... Revisa el discord!")
