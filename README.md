
# MidiaIndoor Player (Android, repo-ready)

- WebView full-screen para `https://midiaindoor.edssmarketing.com.br/public/player.php`
- Autoplay com som, modo imersivo, inicia no boot, opcional kiosk (LockTask se permitido)
- Workflow do GitHub Actions incluso para gerar **APK Debug** automático

## Como gerar APK no GitHub (sem Android Studio)
1. Crie um repositório público no GitHub (ex.: `midiaindoor-player`).
2. Envie o **conteúdo desta pasta** para o repositório (raiz).
   - Via web: abra `https://github.com/<SEU_USUARIO>/<SEU_REPOSITORIO>/upload/main` e arraste os arquivos.
3. Vá em **Actions** → workflow **Android Debug APK** → **Run workflow**.
4. Baixe o **artifact** com o APK em `Actions` → execução → **Artifacts**.

## Personalizar a URL do player
- `app/src/main/res/values/strings.xml` → `<string name="player_url">...</string>`
