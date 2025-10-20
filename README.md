https://github.com/Valroddriguez/chatbot-part2.git #Ella hizo el codigo 2 

aqui ya empezaremos a importar el bot primero descargarlo desde su pagina ollama, terminando esto, podremos ir a cmd o a power shell, aqui para ver que este instalado pondremos esto
ollama serve
al ver que si esta instalado correctamente instalamos la version a utilizar igual en cmd o power pondremos esto
ollama pull qwen2.5:3b #Esperamos a que instale
y para ver que este correctamente usamos el siguiente comando
ollama list
ahora en el codigo para poder usarlo ponemos el servidor a ocupar y la version y importamos librerias como json formato que nos dara el bot, y requets primero para instalarlo pip install requests
y este servira para enviar y recibir datos desde internet o desde un servidor local.

import requests
import json

OLLAMA_URL = "http://localhost:11434/api/generate"
MODEL = "qwen2.5:3b"

y en si esto nos ayudara a poder enviar solicitud de mensajes a ollama y saber que modelo ocupamos, y requets .post para afirmar lo que usamos
