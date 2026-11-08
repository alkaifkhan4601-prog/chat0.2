# Chat to PDF (Android app)

WhatsApp ki exported chat ko WhatsApp jaise interface mein dikhata hai aur PDF bana deta hai. App offline chalta hai, internet permission bhi nahi leta.

## APK banane ke steps (GitHub par, free)

1. github.com par account banao ya login karo.
2. Upar **+** > **New repository** dabao. Naam do (jaise `chat-to-pdf`), **Create repository** karo.
3. Computer par is zip ko extract karo. Repository page par **uploading an existing file** link dabao, aur extract kiye hue folder ke **andar ki sab files aur folders** drag karke daalo (`app`, `.github`, `build.gradle`, `settings.gradle`, `gradle.properties`). Phir **Commit changes**.
4. Upar **Actions** tab kholo. "Build APK" chalta dikhega, 3 se 6 minute lagte hain.
5. Hari tick aane par us run par click karo. Neeche **Artifacts** mein **ChatToPdf-apk** hoga, use download karo. Usme `app-debug.apk` hai.
6. APK ko phone mein bhejo, kholo, aur "Install from unknown sources" allow karo.

## Agar Actions tab mein kuch nahi dikha

`.github` folder hidden hone ki wajah se upload nahi hua hoga. Repository mein **Add file** > **Create new file** dabao, naam mein `.github/workflows/build.yml` likho (slash likhte hi folder ban jata hai), aur is zip ki `.github/workflows/build.yml` file ka text paste karke commit karo.

## Android Studio se banana ho to

Folder ko Android Studio mein kholo, Gradle sync hone do, phir **Build > Build APK(s)**.

## Phone mein use

1. WhatsApp mein chat kholo > teen dots > More > Export chat.
2. File ko apne phone mein save karo (Files / Drive).
3. Chat to PDF kholo, file chuno, "Aap kaun ho?" set karo.
4. **Download PDF** dabao. Print screen mein upar printer ki jagah **Save as PDF** chuno, phir PDF button.
