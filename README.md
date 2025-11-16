     # Jogo Penalti — Pacote Capacitor (pronto para Android)

     Este pacote contém os arquivos web prontos em `www/` com o jogo. Para transformar em APK siga os passos abaixo.

     ## Requisitos
     - Node.js + npm
     - Java JDK (11+)
     - Android Studio (com SDKs Android instalados)

     ## Passos (rápido)
     1. Extraia este ZIP.

     2. No terminal, dentro da pasta do projeto, rode:

```bash
npm install -g @capacitor/cli
npm init -y
npm install @capacitor/core @capacitor/cli
npx cap init
```

     3. Copie os arquivos `www/` para o diretório criado (ou use este repo como `www`).

     4. Adicione a plataforma Android:

```bash
npx cap add android
npx cap copy
npx cap open android
```

     5. O Android Studio vai abrir o projeto. Em seguida: **Build > Build Bundle(s) / APK(s) > Build APK(s)**.

     ## Observações
     - Não consigo compilar o APK neste ambiente. Eu gerei o pacote com tudo que você precisa para abrir no Android Studio e compilar localmente.
     - Se quiser, eu posso incluir um workflow do GitHub Actions para compilar automaticamente (exigirá que você configure chaves/signing e segredos).
