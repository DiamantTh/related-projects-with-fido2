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
- [Fediverse und soziale Netzwerke](categories/fediverse-social.md)
- [Wikis und Wissensmanagement](categories/wikis-knowledge.md)
- [Community und Foren](categories/community-forums.md)

## CMS

Details: [categories/cms.md](categories/cms.md)

| Projekt | Sprache | Impl. | MFA/2FA | Passwordless | Links |
| --- | --- | --- | --- | --- | --- |
| WordPress | PHP | Plugin | Ja | Ja | [Site](https://wordpress.com/de/) [Code](https://github.com/WordPress/WordPress) [2FA](https://de.wordpress.org/plugins/two-factor-provider-webauthn/) [PW](https://de.wordpress.org/plugins/wp-webauthn/) |
| Joomla | PHP | Nativ | Ja | Ja | [Site](https://www.joomla.org/) [Code](https://github.com/joomla/joomla-cms) [PW](https://docs.joomla.org/WebAuthn_Passwordless_Login/en) [MFA](https://docs.joomla.org/J4.x:Multi-factor_Authentication) |

## Code-Hosting und DevOps

Details: [categories/code-hosting-devops.md](categories/code-hosting-devops.md)

| Projekt | Sprache | Impl. | MFA/2FA | Passwordless | Links |
| --- | --- | --- | --- | --- | --- |
| Gitea | Go | Nativ | Ja | Kein Nachweis | [Site](https://about.gitea.com/) [Code](https://github.com/go-gitea/gitea) [Quelle](https://docs.gitea.com/1.23/usage/multi-factor-authentication) |
| GitLab | Ruby | Nativ | Ja | Ja | [Site](https://about.gitlab.com/) [Code](https://gitlab.com/gitlab-org/gitlab) [PW](https://docs.gitlab.com/auth/passkeys/) [MFA](https://docs.gitlab.com/ee/user/profile/account/two_factor_authentication.html) |

## Cloud und Zusammenarbeit

Details: [categories/cloud-collaboration.md](categories/cloud-collaboration.md)

| Projekt | Sprache | Impl. | MFA/2FA | Passwordless | Links |
| --- | --- | --- | --- | --- | --- |
| Nextcloud | PHP | Off. App | Ja | Ja | [Site](https://nextcloud.com/) [Code](https://github.com/nextcloud/server) [2FA-App](https://apps.nextcloud.com/apps/twofactor_webauthn) [PW-Issue](https://github.com/nextcloud/server/issues/51137) [MFA-Hinweis](https://github.com/nextcloud/twofactor_webauthn/issues/475) |

## Identity und Access Management

Details: [categories/identity-access.md](categories/identity-access.md)

| Projekt | Sprache | Impl. | MFA/2FA | Passwordless | Links |
| --- | --- | --- | --- | --- | --- |
| authentik | Python | Nativ | Ja | Ja | [Site](https://goauthentik.io/) [Code](https://github.com/goauthentik/authentik) [WebAuthn](https://docs.goauthentik.io/add-secure-apps/flows-stages/stages/authenticator_webauthn/) [Login](https://docs.goauthentik.io/add-secure-apps/flows-stages/stages/identification/) |
| Keycloak | Java | Nativ | Ja | Ja | [Site](https://www.keycloak.org/) [Code](https://github.com/keycloak/keycloak) [Doku](https://www.keycloak.org/docs/latest/server_admin/) |

## Fediverse und soziale Netzwerke

Details: [categories/fediverse-social.md](categories/fediverse-social.md)

| Projekt | Sprache | Impl. | MFA/2FA | Passwordless | Links |
| --- | --- | --- | --- | --- | --- |
| Mastodon | Ruby | Nativ | Ja | Kein Nachweis | [Site](https://joinmastodon.org/) [Code](https://github.com/mastodon/mastodon) [Issue](https://github.com/mastodon/mastodon/issues/16693) |

## Wikis und Wissensmanagement

Details: [categories/wikis-knowledge.md](categories/wikis-knowledge.md)

| Projekt | Sprache | Impl. | MFA/2FA | Passwordless | Links |
| --- | --- | --- | --- | --- | --- |
| MediaWiki | PHP | Off. Erw. | Ja | Experimentell | [Site](https://www.mediawiki.org/) [Code](https://gerrit.wikimedia.org/g/mediawiki/core) [OATHAuth](https://www.mediawiki.org/wiki/Extension:OATHAuth) |

## Community und Foren

Details: [categories/community-forums.md](categories/community-forums.md)

| Projekt | Sprache | Impl. | MFA/2FA | Passwordless | Links |
| --- | --- | --- | --- | --- | --- |
| Discourse | Ruby | Nativ | Ja | Ja | [Site](https://www.discourse.org/) [Code](https://github.com/discourse/discourse) [PW](https://meta.discourse.org/t/passwordless-login-using-passkeys/285589) [MFA](https://meta.discourse.org/t/locked-out-of-a-discourse-forum-due-to-passkey-bug/362510/8?tl=en) |

## Hinweise zur Einordnung

- `Nativ` bedeutet: Die Funktion ist direkt im Projekt bzw. in dessen offizieller Dokumentation beschrieben.
- `Offizielle App` oder `Offizielle Erweiterung` bedeutet: Nicht im Kern, aber ueber einen offiziell gefuehrten Baustein.
- `Plugins` bedeutet: Die Unterstuetzung ist vorhanden, aber nicht Bestandteil des Kernprojekts.
- `Impl.` ist die Kurzform fuer `Implementierung`.
- `Off. App` und `Off. Erw.` sind Kurzformen fuer `Offizielle App` und `Offizielle Erweiterung`.
- `Kein offizieller Nachweis gefunden` bedeutet nicht zwingend `unmoeglich`, sondern nur, dass hier bewusst nichts behauptet wird, was ich nicht sauber belegen konnte.
- `Ja` in `Passwordless` kann projektabhaengig trotzdem mit weiteren Sicherheitsabfragen kombiniert sein; das ist in den verlinkten Quellen bzw. Issues zu pruefen.
- Die Sprachspalte ist eine grobe Einordnung der Hauptsprache des Projekts.

## Offene und negative Faelle

- `Forgejo` fuehre ich noch nicht separat auf. Dass es aus `Gitea` hervorgegangen ist, ist plausibel fuer aehnliches Verhalten, aber ich habe noch keine direkte Forgejo-Quelle fuer WebAuthn/FIDO2 gefunden. Siehe auch: https://docs.codeberg.org/getting-started/what-is-codeberg/ und https://docs.codeberg.org/security/2fa/
- `Misskey` nehme ich noch nicht in die Haupttabellen auf. Fuer eine belastbare Primärquelle zu WebAuthn/Passkeys habe ich in den offiziellen Misskey-Dokumenten bzw. im offiziellen Projektkontext noch nichts Eindeutiges gefunden.
- `phpBB` hat in der verlinkten Diskussion nur einen Verweis auf eine Erweiterung mit `U2F` und `OTP`; ein belastbarer WebAuthn-Nachweis liegt damit fuer mich noch nicht vor: https://www.phpbb.de/community/viewtopic.php?t=246177
- `MyBB` dokumentiert 2FA allgemein und empfiehlt `U2F` bzw. `TOTP`, aber ich habe auf Basis der offiziellen Doku und des verlinkten Plugins noch keinen belastbaren WebAuthn-Nachweis: https://docs.mybb.com/1.8/administration/security/protection/ und https://www.mybb.de/erweiterungen/18x/plugins-sicherheit/my2fa/
- `WoltLab Suite Core / WCF` fuehre ich nicht in den Haupttabellen. Aktuell sehe ich ein offenes Ticket zur nativen Umsetzung und ausserhalb davon vor allem ein separates Plugin, nicht belastbar als Core-Support: https://github.com/WoltLab/WCF/issues/6440 und https://www.woltlab.com/pluginstore/file/3101-webauthn-login/

## Lizenz

Die Inhalte dieses Repos stehen unter `Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)`.

- Lizenztext: [LICENSE.md](LICENSE.md)
- Offizielle Lizenz: https://creativecommons.org/licenses/by-sa/4.0/

---

Hinweis: Diese Markdown-Datei wurde mit Unterstuetzung von KI erstellt und anschliessend anhand der verlinkten Quellen strukturiert. Sofern nicht anders angegeben, stehen die Texte und Listen in diesem Repo unter CC BY-SA 4.0. Fehler, veraltete Angaben oder fehlende Projekte bitte per Issue oder Pull Request melden.
