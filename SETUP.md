# TNHRA website – one-time setup (for Vikas)

All accounts below must be created with TNHRA email addresses, never personal ones.

## 1. Domain and email
1. Buy the domain (tnhra.com) in TNHRA's name.
2. Set up email on it (Zoho Mail or Google Workspace): president@tnhra.com , secretary@, treasurer@, info@.
3. Keep one owner login (e.g. admin@ or info@) with its password and recovery codes in a sealed note with the President.

## 2. GitHub (stores the website files)
1. Create a free GitHub account with president@tnhra.com.
2. Create an repository "tnhra-website" (account: tnhraorg-wq).
3. Upload everything in this folder to that repository (Add file → Upload files).
4. If you used a different organisation/repository name, change the `repo:` line in admin/config.yml.

## 3. Netlify (puts the website online, free)
1. Sign up at netlify.com with "Log in with GitHub" (the info@ account).
2. Add new site → Import from GitHub → choose tnhra-website → Deploy. No build settings are needed.
3. Domain management → Add your domain (tnhra.com) and follow the DNS steps shown.
4. Admin login: In GitHub, Settings → Developer settings → OAuth Apps → New OAuth App.
   - Homepage URL: https://tnhra.com
   - Callback URL: https://api.netlify.com/auth/done
   Copy the Client ID and Secret. In Netlify: Site configuration → Access & security → OAuth → Install provider → GitHub, paste them.

## 4. Give the Secretary access
1. Secretary creates a free GitHub account using secretary@tnhra.com.
2. In the tnhra-org organisation → People → Invite → add that account with **Write** access to tnhra-website.
3. Do the same for president@tnhra.com .
4. Secretary opens https://tnhra.com/admin → "Login with GitHub".

## When office bearers change
- Hand over the secretary@ mailbox: change its password and recovery phone.
- On github.com with that email, use "Forgot password" to reset it, then turn on 2-step verification with the new person's phone.
- Nothing else changes; the access stays with the post, not the person.

## Notes
- Every change is saved with a history, so mistakes can be undone from GitHub.
- Riders' private data (parents' contacts, dates of birth) is NOT in this website. Keep it in TNHRA's own records only.
- The EFI 12-hour auto-check currently updates the old Claude page. Once this site is live, ask Claude to switch it to update data/efi_posts.json.
