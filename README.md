# ComZap
Sistema de atendimento automático desenvolvido por Werley 💬✨

Primeiro commit do ComZap
cd /www/wwwroot/jwartesdig.com.br/comzap && \
mkdir -p bootstrap routes resources/views && \
echo "#!/usr/bin/env php\n<?php\n\nrequire __DIR__.'/bootstrap/app.php';\n\necho \"Artisan mock iniciado\\n\";" > artisan && \
chmod +x artisan && \
echo "<?php\n\n\$app = [];\n\nreturn \$app;" > bootstrap/app.php && \
echo "<?php\n\nuse Illuminate\\Support\\Facades\\Route;\n\nRoute::get('/', function () {\n    return view('welcome');\n});" > routes/web.php && \
echo "<!DOCTYPE html>\n<html>\n<head>\n    <title>ComZap Funcionando!</title>\n</head>\n<body>\n    <h1>Bem-vindo ao ComZap 🚀</h1>\n    <p>Sistema online com sucesso!</p>\n</body>\n</html>" > resources/views/welcome.blade.php && \
echo "APP_NAME=ComZap\nAPP_ENV=local\nAPP_KEY=\nAPP_DEBUG=true\nAPP_URL=http://localhost\n\nDB_CONNECTION=mysql\nDB_HOST=127.0.0.1\nDB_PORT=3306\nDB_DATABASE=comzap\nDB_USERNAME=root\nDB_PASSWORD=senhaSegura123" > .env.example && \
echo "{\n  \"name\": \"comzap/laravel\",\n  \"require\": {\n    \"php\": \">=7.3\",\n    \"laravel/framework\": \"^8.0\"\n  }\n}" > composer.json
