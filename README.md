# FOSS mit FIDO2

Diese Sammlung dokumentiert den aktuellen Stand von FOSS-Projekten und offenen Plattformen, die FIDO2, WebAuthn, Passkeys oder Hardware-Sicherheitsschluessel unterstuetzen. Aufgenommen werden nur Eintraege, fuer die sich die Unterstuetzung anhand belastbarer Quellen nachvollziehen laesst, bevorzugt ueber offizielle Dokumentation, offizielle Projektseiten oder offizielle Erweiterungen.

Die Trennung zwischen `MFA/2FA` und `Passwordless` ist absichtlich strikt:

- `MFA/2FA` bedeutet: WebAuthn/FIDO2 wird als zweiter Faktor nach Passwort verwendet.
- `Passwordless` bedeutet: Anmeldung ohne Passwort per Passkey, WebAuthn oder vergleichbarem FIDO2-Flow.
- Wenn nur Plugin- oder Erweiterungs-Support existiert, wird das in `Implementierung` explizit genannt.

## Kategorien

- [CMS](categories/cms.md)
- [Code-Hosting und DevOps](categories/code-hosting-devops.md)
- [Cloud und Zusammenarbeit](categories/cloud-collaboration.md)
- [Identity und Access Management](categories/identity-access.md)
- [Wikis und Wissensmanagement](categories/wikis-knowledge.md)
- [Community und Foren](categories/community-forums.md)

## Starttabelle

| Projekt | Website | Quellcode | Kategorie | Hauptsprache | Implementierung | MFA/2FA | Passwordless | Quelle |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| WordPress | https://wordpress.com/de/ | https://github.com/WordPress/WordPress | CMS | PHP | Plugins | Ja, per Two-Factor WebAuthn Provider | Ja, per WP-WebAuthn | https://de.wordpress.org/plugins/two-factor-provider-webauthn/ ; https://de.wordpress.org/plugins/wp-webauthn/ |
| Joomla | https://www.joomla.org/ | https://github.com/joomla/joomla-cms | CMS | PHP | Core / offizielle Doku | Ja, WebAuthn kann auch als zweiter Faktor genutzt werden | Ja, ueber System - WebAuthn Passwordless Login | https://docs.joomla.org/WebAuthn_Passwordless_Login/en ; https://docs.joomla.org/J4.x:Multi-factor_Authentication |
| Gitea | https://about.gitea.com/ | https://github.com/go-gitea/gitea | Code-Hosting und DevOps | Go | Nativ | Ja, FIDO-basierte Hardware-Keys via WebAuthn | Kein offizieller Nachweis gefunden | https://docs.gitea.com/1.23/usage/multi-factor-authentication |
| GitLab | https://about.gitlab.com/ | https://gitlab.com/gitlab-org/gitlab | Code-Hosting und DevOps | Ruby | Nativ | Ja, WebAuthn Devices oder Passkeys als 2FA | Ja, Passkey Sign-in | https://docs.gitlab.com/auth/passkeys/ ; https://docs.gitlab.com/ee/user/profile/account/two_factor_authentication.html |
| Nextcloud | https://nextcloud.com/ | https://github.com/nextcloud/server | Cloud und Zusammenarbeit | PHP | Offizielle App | Ja, ueber Two-Factor WebAuthn | Kein offizieller Nachweis gefunden | https://apps.nextcloud.com/apps/twofactor_webauthn ; https://docs.nextcloud.com/server/26/admin_manual/configuration_user/two_factor-auth.html |
| authentik | https://goauthentik.io/ | https://github.com/goauthentik/authentik | Identity und Access Management | Python | Nativ | Ja | Ja | https://docs.goauthentik.io/add-secure-apps/flows-stages/stages/authenticator_webauthn/ ; https://docs.goauthentik.io/add-secure-apps/flows-stages/stages/identification/ |
| Keycloak | https://www.keycloak.org/ | https://github.com/keycloak/keycloak | Identity und Access Management | Java | Nativ | Ja, WebAuthn als 2FA | Ja, passwordless und loginless WebAuthn / Passkeys | https://www.keycloak.org/docs/latest/server_admin/ |
| MediaWiki | https://www.mediawiki.org/ | https://gerrit.wikimedia.org/g/mediawiki/core | Wikis und Wissensmanagement | PHP | Offizielle Erweiterung | Ja, Passkeys und Security Keys ueber OATHAuth | Experimentell, ueber OATHAuth | https://www.mediawiki.org/wiki/Extension:OATHAuth |
| Discourse | https://www.discourse.org/ | https://github.com/discourse/discourse | Community und Foren | Ruby | Nativ | Ja, Security Keys als Second Factor laut Discourse Meta Team | Ja, Passkeys seit 2023 | https://meta.discourse.org/t/passwordless-login-using-passkeys/285589 ; https://meta.discourse.org/t/locked-out-of-a-discourse-forum-due-to-passkey-bug/362510/8?tl=en |

## Hinweise zur Einordnung

- `Nativ` bedeutet: Die Funktion ist direkt im Projekt bzw. in dessen offizieller Dokumentation beschrieben.
- `Offizielle App` oder `Offizielle Erweiterung` bedeutet: Nicht im Kern, aber ueber einen offiziell gefuehrten Baustein.
- `Plugins` bedeutet: Die Unterstuetzung ist vorhanden, aber nicht Bestandteil des Kernprojekts.
- `Kein offizieller Nachweis gefunden` bedeutet nicht zwingend `unmoeglich`, sondern nur, dass hier bewusst nichts behauptet wird, was ich nicht sauber belegen konnte.
- Die Sprachspalte ist eine grobe Einordnung der Hauptsprache des Projekts.

---

Hinweis: Diese Markdown-Datei wurde mit Unterstuetzung von KI erstellt und anschliessend anhand der verlinkten Quellen strukturiert. Fehler, veraltete Angaben oder fehlende Projekte bitte per Issue oder Pull Request melden.
