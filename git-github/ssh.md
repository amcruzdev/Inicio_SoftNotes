### Comandos del protocolo SSH 
1. `ssh-keygen -t rsa -b 4096 -C "correo"`<p>Genera un par de llaves asimetricas</p>
2. `eval $(ssh-agent -s)`<p>Brinda el agent PID, para confirmar que la llave este corriendo</p>
3. `ssh-add <ruta_llavePrivada>`<p>Agregamos la llaves a ssh-agent</p>