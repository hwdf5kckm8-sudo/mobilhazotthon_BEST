Render deploy lépések

1. Hozd létre a GitHub repót és pushold fel a projektet:
   - git init
   - git branch -M main
   - git add .
   - git commit -m "Initial commit — mobilhaz site"
   - git remote add origin git@github.com:<your-username>/mobilhaz.git
   - git push -u origin main

2. Jelentkezz be a Render.com fiókodba (vagy regisztrálj): https://dashboard.render.com
3. Új szolgáltatás létrehozása: "New" → "Static Site" → "Connect a repo"
   - Válaszd ki a GitHub repo-d, és válaszd a `main` branch-et.
   - Build Command: hagyd üresen (nincs build).
   - Publish directory: `.` (a repo gyökere).
   - Create Static Site.

4. Várd meg a deploy befejezését — Render ad egy publikus URL-t.

Tippek / Hibakezelés
- Ha privát repo-t használsz, engedélyezd a Render-nek a hozzáférést GitHub-on keresztül.
- Ha módosítod a képeket/fájlokat, commit/ push → Render automatikusan újra deploy-olja.

Ha szeretnéd, segítek a `git push`-ban (ha megadod a GitHub repo-URL-t), vagy végigvezetlek a Render UI lépésein.