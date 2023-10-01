# Hook Send

Este script de python tiene la función de enviar una petición de mensaje a una Webhook de Discord

## Capturas
![Main](https://cdn.discordapp.com/attachments/1006331564927500318/1158179811945099365/image.png?ex=651b4e81&is=6519fd01&hm=b13a6314fa30e25b1341beab0da46b3b7dab3a89705fda1c91557d46563ab148&)
![DiscordMain](https://cdn.discordapp.com/attachments/1006331564927500318/1158179812150628462/image.png?ex=651b4e81&is=6519fd01&hm=9c4fd9b040f009a3616a939e2c324aec89e5cb81dda72bad584eb58ddf6e3dcf&)

## Ejecutar

> **⚠ Editar la linea 6 con tu URL de WebHook**

> Windows
> 
> ```python -m pip install -r requirements.txt```
> ```python hooksend.py```

> Linux
> 
> ```git clone https://github.com/KaltHack/HookSend```
> ```cd HookSend```
> ```python3 -m pip install -r requirements.txt```
> ```python3 hooksend.py```

## Censura de links

El script tiene un filtro para que no se puedan enviar enlaces ni en el nombre ni en el mensaje del Webhook
![Ban](https://media.discordapp.net/attachments/1006331564927500318/1158179812595208253/image.png?ex=651b4e81&is=6519fd01&hm=e2b13f1f8464a08d3bb8a2118f0f015ec3f7ac7c8d04f4737ed55d31efeefa66&=&width=417&height=137)

