# Mercadinho Oliveira - APK Android

Este repositório gera um APK Android que abre o sistema online:

https://mercadinho-lxyl.onrender.com/

## Estrutura correta no GitHub

Na raiz do repositório devem existir:

- `.github/workflows/build-apk.yml`
- `mercadinho-oliveira-apk-android/`

Dentro da pasta `mercadinho-oliveira-apk-android` ficam os arquivos Android: `app/`, `build.gradle`, `settings.gradle` etc.

## Gerar APK

1. Envie estes arquivos para o GitHub.
2. Vá na aba **Actions**.
3. Abra **Gerar APK Android**.
4. Clique em **Run workflow**.
5. Quando terminar, abra o run concluído e baixe o artefato **Mercadinho-Oliveira-APK**.

## Observação

Este projeto não usa `./gradlew`. O workflow instala o Gradle automaticamente no GitHub Actions.
