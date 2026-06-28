# Mercadinho Oliveira - APK Android

Este projeto gera um aplicativo Android que abre o sistema online:

https://mercadinho-lxyl.onrender.com/

O site continua funcionando normalmente no Render. O APK funciona como um app no celular, usando o mesmo Supabase e os mesmos dados.

## Forma 1: gerar APK pelo GitHub Actions

1. Crie um novo repositório no GitHub, por exemplo: `mercadinho-oliveira-apk`.
2. Envie todos os arquivos deste projeto para o repositório.
3. No GitHub, entre em **Actions**.
4. Abra o workflow **Gerar APK Android**.
5. Clique em **Run workflow**.
6. Ao terminar, baixe o artefato **Mercadinho-Oliveira-APK**.
7. O arquivo será `app-debug.apk`.
8. Envie o APK para seu celular e instale.

No Android, pode ser necessário permitir instalação de apps de fontes desconhecidas.

## Forma 2: gerar APK pelo Android Studio

1. Instale o Android Studio.
2. Abra este projeto.
3. Espere o Gradle sincronizar.
4. Clique em **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. O APK será gerado em:

`app/build/outputs/apk/debug/app-debug.apk`

## Observações importantes

- O app precisa de internet, pois ele abre o sistema hospedado no Render.
- A câmera foi habilitada para o leitor de código de barras do PDV.
- O login e os dados continuam no Supabase.
- Quando você atualizar o site no Render, o app abrirá a versão atualizada automaticamente.
- Se mudar a URL do site, altere o arquivo `app/src/main/res/values/strings.xml`.
