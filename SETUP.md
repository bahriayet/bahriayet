# GitHub profile — remaining manual steps

Most of the cleanup is already live. This file lists only the steps that need
your GitHub login.

## Already done

- Profile repository `bahriayet/bahriayet` created with a black-and-neon-green
  README, animated banner, typing header, project cards, and GitHub summary
  cards.
- `busa` has a new README, MIT license, CI, issue templates, Dependabot, and
  security settings.
- `portofolioku`, `undanga-pernikahan`, `KICK-STORM`, and
  `smart-facility-hub` have new READMEs, metadata, and topics.
- `KICK-STORM` was rebuilt as a clean public repository. The old repository is
  private and archived as `kickstorm-archive`.
- `hehe1` (old WhatsApp bot code) is private and archived.
- `Hehe-123` was renamed to `symbiotrade-spec` and given a proper README.
- Repository descriptions, topics, and homepages were updated through the API.

## 1. Set the profile details

Open <https://github.com/settings/profile>.

**Profile picture**

Upload `D:\ui-profile\assets\avatar.png` (black-and-neon-green BM monogram).

**Bio**

```text
Full-stack developer · TypeScript, Fastify, PostgreSQL · Building production tools for small businesses in Indonesia.
```

**Website**

```text
https://portofolioku-ochre-nu.vercel.app
```

**Location**

```text
Mataram, Indonesia
```

## 2. Pin repositories

Open <https://github.com/bahriayet> and click **Customize your pins**.

Pin, in this order:

1. `busa`
2. `KICK-STORM`
3. `portofolioku`
4. `undanga-pernikahan`
5. `symbiotrade-spec`
6. `smart-facility-hub`

Pinning replaces the default "Popular repositories" list, which is currently
ordered by GitHub's own logic.

## 3. Social preview images

For `busa`: **Settings → General → Social preview → Upload an image**.
Use `D:\ui\docs\screenshots\landing-desktop.png` (crop to 1280×640).

For the profile repository: upload `D:\ui-profile\assets\banner.png`.

## 4. Rotate the exposed admin password

The old `KICK-STORM` repository publicly exposed `.env.example` with an admin
password and a database backup with customer names, emails, and addresses.

1. Change `ADMIN_PASSWORD` in the deployment environment (Vercel/Render).
2. Redeploy so the new password takes effect.
3. Confirm the old admin tokens no longer work. Tokens are signed with the
   admin password, so rotating it invalidates them.
4. Delete the `kickstorm-archive` repository once you no longer need it:
   **Settings → General → Danger Zone → Delete this repository**.

The new `KICK-STORM` repository has no database backups, uploads, or real
password in its history.

## 5. Optional

- Enable 2FA: <https://github.com/settings/security>.
- Review the six Dependabot pull requests on `busa`; merge or close them.
- Add a profile photo if the current avatar is not the one you want.
- Add a LinkedIn or personal domain to the profile links.
