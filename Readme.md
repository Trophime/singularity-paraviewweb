web/htdocs: contient index.html

singularity instance start -B web/htdocs:/var/www/html apache.simg apache2
singularity shell instance://apache2
nmap localhost
w3m http://localhost:8080