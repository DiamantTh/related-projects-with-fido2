# FOSS mit FIDO2

Lizenz der Repo-Texte und Tabellen: [CC BY-SA 4.0](LICENSE.md)

Diese Sammlung dokumentiert den aktuellen Stand von FOSS-Projekten und offenen Plattformen, die FIDO2, WebAuthn, Passkeys oder Hardware-Sicherheitsschluessel unterstuetzen. Aufgenommen werden nur Eintraege, fuer die sich die Unterstuetzung anhand belastbarer Quellen nachvollziehen laesst, bevorzugt ueber offizielle Dokumentation, offizielle Projektseiten oder offizielle Erweiterungen.

Die Trennung zwischen `MFA/2FA` und `Passwordless` ist absichtlich strikt:

- `MFA/2FA` bedeutet: WebAuthn/FIDO2 wird als zweiter Faktor nach Passwort verwendet.
- `Passwordless` bedeutet: Anmeldung ohne Passwort per Passkey, WebAuthn oder vergleichbarem FIDO2-Flow.
- Wenn nur Plugin- oder Erweiterungs-Support existiert, wird das in `Implementierung` explizit genannt.

## Kategorien

- [Cloud und Zusammenarbeit](categories/cloud-collaboration.md)
- [CMS](categories/cms.md)
- [Code-Hosting und DevOps](categories/code-hosting-devops.md)
- [Community und Foren](categories/community-forums.md)
- [DNS- und Infrastruktur-Panels](categories/dns-infra-panels.md)
- [Fediverse und soziale Netzwerke](categories/fediverse-social.md)
- [Identity und Access Management](categories/identity-access.md)
- [Server- und Hosting-Panels](categories/server-hosting-panels.md)
- [Ticketsysteme und Helpdesk](categories/ticketing-helpdesk.md)
- [Wikis und Wissensmanagement](categories/wikis-knowledge.md)

## Cloud und Zusammenarbeit

Details: [categories/cloud-collaboration.md](categories/cloud-collaboration.md)

| Projekt | Sprache | Impl. | MFA/2FA | Passwordless | Ausblick | Links |
| --- | --- | --- | --- | --- | --- | --- |
| Nextcloud | PHP | Off. App | Ja | Ja | Vorhanden | [Site](https://nextcloud.com/) [Code](https://github.com/nextcloud/server) [2FA-App](https://apps.nextcloud.com/apps/twofactor_webauthn) [PW-Issue](https://github.com/nextcloud/server/issues/51137) [MFA-Hinweis](https://github.com/nextcloud/twofactor_webauthn/issues/475) |

## CMS

Details: [categories/cms.md](categories/cms.md)

| Projekt | Sprache | Impl. | MFA/2FA | Passwordless | Ausblick | Links |
| --- | --- | --- | --- | --- | --- | --- |
| Drupal | PHP | Modul | Kein Nachweis | Ja | Per Modul vorhanden | [Site](https://www.drupal.org/) [Code](https://git.drupalcode.org/project/drupal) [PW](https://www.drupal.org/project/wa) |
| Ghost | JavaScript | Kein Nachweis | Kein Nachweis | Kein Nachweis | Kein Hinweis | [Site](https://ghost.org/) [Code](https://github.com/TryGhost/Ghost) [Docs](https://docs.ghost.org/) |
| Grav | PHP | Kein Nachweis | Kein Nachweis | Kein Nachweis | Offen | [Site](https://getgrav.org/) [Code](https://github.com/getgrav/grav) [Issue](https://github.com/getgrav/grav/issues/3919) |
| Joomla | PHP | Nativ | Ja | Ja | Vorhanden | [Site](https://www.joomla.org/) [Code](https://github.com/joomla/joomla-cms) [PW](https://docs.joomla.org/WebAuthn_Passwordless_Login/en) [MFA](https://docs.joomla.org/J4.x:Multi-factor_Authentication) |
| TYPO3 | PHP | Erweiterung | Kein Nachweis | Ja | Per Erweiterung vorhanden | [Site](https://typo3.org/) [Code](https://github.com/TYPO3/typo3) [BE](https://docs.typo3.org/p/netresearch/nr-passkeys-be/main/en-us/) [FE](https://docs.typo3.org/p/netresearch/nr-passkeys-fe/main/en-us) |
| WordPress | PHP | Plugin | Ja | Ja | Per Plugin vorhanden | [Site](https://wordpress.com/de/) [Code](https://github.com/WordPress/WordPress) [2FA](https://de.wordpress.org/plugins/two-factor-provider-webauthn/) [PW](https://de.wordpress.org/plugins/wp-webauthn/) |

## Code-Hosting und DevOps

Details: [categories/code-hosting-devops.md](categories/code-hosting-devops.md)

| Projekt | Sprache | Impl. | MFA/2FA | Passwordless | Ausblick | Links |
| --- | --- | --- | --- | --- | --- | --- |
| Forgejo | Go | Nativ* | Ja* | Kein Nachweis | Teilweise vorhanden | [Site](https://forgejo.org/) [Info](https://docs.codeberg.org/getting-started/what-is-codeberg/) [2FA](https://docs.codeberg.org/security/2fa/) |
| Gitea | Go | Nativ | Ja | Kein Nachweis | Teilweise vorhanden | [Site](https://about.gitea.com/) [Code](https://github.com/go-gitea/gitea) [Quelle](https://docs.gitea.com/1.23/usage/multi-factor-authentication) |
| GitLab | Ruby | Nativ | Ja | Ja | Vorhanden | [Site](https://about.gitlab.com/) [Code](https://gitlab.com/gitlab-org/gitlab) [PW](https://docs.gitlab.com/auth/passkeys/) [MFA](https://docs.gitlab.com/ee/user/profile/account/two_factor_authentication.html) |

## Community und Foren

Details: [categories/community-forums.md](categories/community-forums.md)

| Projekt | Sprache | Impl. | MFA/2FA | Passwordless | Ausblick | Links |
| --- | --- | --- | --- | --- | --- | --- |
| Discourse | Ruby | Nativ | Ja | Ja | Vorhanden | [Site](https://www.discourse.org/) [Code](https://github.com/discourse/discourse) [PW](https://meta.discourse.org/t/passwordless-login-using-passkeys/285589) [MFA](https://meta.discourse.org/t/locked-out-of-a-discourse-forum-due-to-passkey-bug/362510/8?tl=en) |
| Flarum | PHP | Plugin | Kein Nachweis | Ja | Per Plugin vorhanden | [Site](https://flarum.org/) [Code](https://github.com/flarum/framework) [PW](https://flarum.org/extension/hikarilan/flarum-passkey-login) [Thread](https://discuss.flarum.org/d/33682-passkey-login) |
| NodeBB | JavaScript | Off. Plugin | Ja | Kein Nachweis | Teilweise vorhanden | [Site](https://nodebb.org/) [Code](https://github.com/NodeBB/NodeBB) [Blog](https://nodebb.org/blog/fido2-webauthn) [Plugin](https://www.npmjs.com/package/nodebb-plugin-2factor) |
| WoltLab Suite Core / WCF | PHP | Kommerzielles Plugin | Kein Nachweis | Ja | Geplant | [Site](https://www.woltlab.com/) [Code](https://github.com/WoltLab/WCF) [Plugin](https://www.woltlab.com/pluginstore/file/3101-webauthn-login/) [Issue](https://github.com/WoltLab/WCF/issues/6440) |

## DNS- und Infrastruktur-Panels

Details: [categories/dns-infra-panels.md](categories/dns-infra-panels.md)

| Projekt | Sprache | Impl. | MFA/2FA | Passwordless | Ausblick | Links |
| --- | --- | --- | --- | --- | --- | --- |
| Poweradmin | PHP | Nativ | Nein (nur TOTP) | Kein Nachweis | Kein Hinweis | [Site](https://www.poweradmin.org/) [Code](https://github.com/poweradmin/poweradmin) [Auth](https://github.com/poweradmin/poweradmin) |
| PowerDNS-Admin | Python | Nativ | Nein (nur TOTP) | Kein Nachweis | Kein Hinweis | [Site](https://powerdnsadmin.org) [Code](https://github.com/PowerDNS-Admin/PowerDNS-Admin) [Auth](https://github.com/PowerDNS-Admin/PowerDNS-Admin) |

## Fediverse und soziale Netzwerke

Details: [categories/fediverse-social.md](categories/fediverse-social.md)

| Projekt | Sprache | Impl. | MFA/2FA | Passwordless | Ausblick | Links |
| --- | --- | --- | --- | --- | --- | --- |
| Akkoma | Elixir | Kein Nachweis | Kein Nachweis | Kein Nachweis | Offen | [Site](https://akkoma.dev/) [Code](https://akkoma.dev/AkkomaGang/akkoma) [Issue](https://akkoma.dev/AkkomaGang/akkoma/issues/608) |
| Mastodon | Ruby | Nativ | Ja | Kein Nachweis | Offen | [Site](https://joinmastodon.org/) [Code](https://github.com/mastodon/mastodon) [Issue](https://github.com/mastodon/mastodon/issues/16693) |
| Misskey | TypeScript | Nativ | Ja | Ja | Vorhanden | [Site](https://misskey-hub.net/en/) [Code](https://github.com/misskey-dev/misskey) [Frontend](https://github.com/misskey-dev/misskey/blob/develop/packages/frontend/src/components/MkSignin.vue) [2FA-UI](https://github.com/misskey-dev/misskey/blob/develop/packages/frontend/src/pages/settings/2fa.vue) [Backend](https://github.com/misskey-dev/misskey/blob/develop/packages/backend/src/core/WebAuthnService.ts) [E2E](https://github.com/misskey-dev/misskey/blob/develop/packages/backend/test/e2e/2fa.ts) |

## Identity und Access Management

Details: [categories/identity-access.md](categories/identity-access.md)

| Projekt | Sprache | Impl. | MFA/2FA | Passwordless | Ausblick | Links |
| --- | --- | --- | --- | --- | --- | --- |
| authentik | Python | Nativ | Ja | Ja | Vorhanden | [Site](https://goauthentik.io/) [Code](https://github.com/goauthentik/authentik) [WebAuthn](https://docs.goauthentik.io/add-secure-apps/flows-stages/stages/authenticator_webauthn/) [Login](https://docs.goauthentik.io/add-secure-apps/flows-stages/stages/identification/) |
| Keycloak | Java | Nativ | Ja | Ja | Vorhanden | [Site](https://www.keycloak.org/) [Code](https://github.com/keycloak/keycloak) [Doku](https://www.keycloak.org/docs/latest/server_admin/) |

## Server- und Hosting-Panels

Details: [categories/server-hosting-panels.md](categories/server-hosting-panels.md)

| Projekt | Sprache | Impl. | MFA/2FA | Passwordless | Ausblick | Links |
| --- | --- | --- | --- | --- | --- | --- |
| Froxlor | PHP | Kein Nachweis | Kein Nachweis | Kein Nachweis | Offen | [Site](https://froxlor.org/) [Code](https://github.com/Froxlor/Froxlor) [Issue](https://github.com/Froxlor/Froxlor/issues/1281) [2FA-Datei](https://github.com/Froxlor/Froxlor/blob/main/2fa.php) [Docs](https://docs.froxlor.org/) |
| HestiaCP | Shell/PHP | Kein Nachweis | Kein Nachweis | Kein Nachweis | Kein Hinweis | [Site](https://hestiacp.com/) [Code](https://github.com/hestiacp/hestiacp) |
| ISPConfig | PHP | Kein Nachweis | Kein Nachweis | Kein Nachweis | Kein Hinweis | [Site](https://www.ispconfig.org/) [Docs](https://www.ispconfig.org/documentation/) |
| Portainer CE | TypeScript/Go | Kein Nachweis | Kein Nachweis | Kein Nachweis | Kein Hinweis | [Site](https://www.portainer.io/) [Code](https://github.com/portainer/portainer) [Docs](https://docs.portainer.io/) |
| Proxmox VE | Perl/JavaScript | Nativ | Ja | Kein Nachweis | Teilweise vorhanden | [Site](https://www.proxmox.com/en/proxmox-virtual-environment/overview) [Code](https://github.com/proxmox) [WebAuthn](https://pve.proxmox.com/pve-docs/chapter-pveum.html) |
| Virtualmin GPL | Perl | Kein Nachweis | Kein Nachweis | Kein Nachweis | Kein Hinweis | [Site](https://www.virtualmin.com/) [Info](https://webmin.com/virtualmin/) |
| Webmin | Perl | Nativ | Nein (nur TOTP) | Kein Nachweis | Kein Hinweis | [Site](https://webmin.com/) [Code](https://github.com/webmin/webmin) [2FA](https://webmin.com/docs/modules/webmin-configuration) |

## Ticketsysteme und Helpdesk

Details: [categories/ticketing-helpdesk.md](categories/ticketing-helpdesk.md)

| Projekt | Sprache | Implementierung | MFA/2FA | Passwordless | Ausblick | Links |
| --- | --- | --- | --- | --- | --- | --- |
| FreeScout | PHP | Offizielles SAML-Modul | Kein nativer Nachweis | Indirekt via offiziellem SAML-Modul | Kein Hinweis | [Site](https://freescout.net/) [Code](https://github.com/freescout-help-desk/freescout) [Module](https://github.com/freescout-help-desk/freescout/wiki/FreeScout-Modules) [SAML](https://freescout.net/module/saml/) [Git-Issue](https://github.com/freescout-help-desk/freescout/issues) |
| GLPI | PHP | Offizielle OAuth-/SAML-Plugins | Kein nativer Nachweis | Indirekt via OAuth SSO oder SAML | Kein Hinweis | [Site](https://glpi-project.org/) [Code](https://github.com/glpi-project/glpi) [Core-Auth](https://help.glpi-project.org/documentation/modules/configuration/authentication) [OAuth](https://help.glpi-project.org/doc-plugins/oauthsso) [SAML](https://help.glpi-project.org/doc-plugins/plugins-glpi/saml) |
| osTicket | PHP | Klassische Auth / Plugins | Kein Nachweis | Kein Nachweis | Kein Hinweis | [Site](https://osticket.com/) [Code](https://github.com/osTicket/osTicket) [Docs](https://docs.osticket.com/) [Plugins](https://github.com/osTicket/osTicket-plugins) |
| OTOBO | Perl | Klassische Auth | Kein Nachweis | Kein Nachweis | Kein Hinweis | [Site](https://otobo.de/en/) [Code](https://github.com/RotherOSS/otobo) [Auth](https://doc.otobo.org/manual/developer/10.1/en/content/how-to-extend-otobo/otobo-module-layers/auth-sync.html) |
| Request Tracker (RT) | Perl | Externe Webserver-Auth | Kein nativer Nachweis | Indirekt ueber externen Webserver/Auth-Stack | Kein Hinweis | [Site](https://bestpractical.com/request-tracker) [Code](https://github.com/bestpractical/rt) [Auth](https://docs.bestpractical.com/rt/5.0.9/authentication.html) |
| Zammad | Ruby | Kerberos-SSO | Kein nativer Nachweis | Indirekt via Kerberos-SSO | Kein Hinweis | [Site](https://zammad.com/) [Code](https://github.com/zammad/zammad) [SSO](https://docs.zammad.org/en/latest/appendix/single-sign-on.html) |
| Znuny | Perl | Eingebautes SAML-SSO | Kein nativer Nachweis | Indirekt via SAML-IdP | Kein Hinweis | [Site](https://www.znuny.com/) [Code](https://github.com/znuny/Znuny) [SAML](https://www.znuny.com/blog/znuny-built-in-saml-authentication) |

## Wikis und Wissensmanagement

Details: [categories/wikis-knowledge.md](categories/wikis-knowledge.md)

| Projekt | Sprache | Impl. | MFA/2FA | Passwordless | Ausblick | Links |
| --- | --- | --- | --- | --- | --- | --- |
| MediaWiki | PHP | Off. Erw. | Ja | Experimentell | Teilweise vorhanden | [Site](https://www.mediawiki.org/) [Code](https://gerrit.wikimedia.org/g/mediawiki/core) [OATHAuth](https://www.mediawiki.org/wiki/Extension:OATHAuth) |

## Hinweise zur Einordnung

- `Nativ` bedeutet: Die Funktion ist direkt im Projekt bzw. in dessen offizieller Dokumentation beschrieben.
- `Offizielle App` oder `Offizielle Erweiterung` bedeutet: Nicht im Kern, aber ueber einen offiziell gefuehrten Baustein.
- `Plugins` bedeutet: Die Unterstuetzung ist vorhanden, aber nicht Bestandteil des Kernprojekts.
- `SSO/IdP` bedeutet: Die Anmeldung kann ueber ein externes Identitaetssystem laufen; FIDO2/Passkeys haengen dann vom angebundenen IdP ab, nicht vom Projekt selbst.
- `Plugin/SSO` bedeutet: Die Funktion kommt ueber ein offizielles oder etabliertes Zusatzmodul und haengt oft ebenfalls am externen IdP.
- `Ausblick` beschreibt den praktisch nuetzlichen Status fuer die Weiterentwicklung oder Vollstaendigkeit des FIDO2/WebAuthn-Supports.
- `Vorhanden` bedeutet: Das Projekt hat den benoetigten Support bereits in der geprueften Form.
- `Teilweise vorhanden` bedeutet: Ein Teil des Supports ist da, z. B. nur MFA/2FA, aber nicht klar passwordless.
- `Per Plugin vorhanden` oder `Per Erweiterung vorhanden` bedeutet: Die Funktion ist verfuegbar, aber nicht nativ im Kern.
- `Geplant` bedeutet: Es gibt einen konkreten Hinweis, dass WebAuthn/FIDO2/Passkeys kommen sollen, auch wenn es noch nicht verfuegbar ist.
- `Offen` bedeutet: Es gibt eine erkennbare Diskussion, ein Feature-Request oder eine laufende Richtung.
- `Kein Nachweis` bedeutet: In den geprueften offiziellen Quellen habe ich fuer WebAuthn/FIDO2/Passkeys keinen belastbaren Beleg gefunden.
- `Nein (nur TOTP)` bedeutet: Offiziell belegt ist klassische 2FA, aber nicht WebAuthn/FIDO2/Passkeys.
- `Unklar` bedeutet: Im Projekt gibt es eine technische Spur, aber noch keinen sauberen belastbaren Nachweis, wie weit WebAuthn/FIDO2 wirklich getragen wird.
- `Repo-Spur` bedeutet: Im offiziellen Quellcode ist ein deutlicher Auth-/2FA-Hinweis sichtbar, aber die offizielle Doku reicht fuer eine scharfe Einordnung noch nicht aus.
- `Impl.` ist die Kurzform fuer `Implementierung`.
- `Off. App` und `Off. Erw.` sind Kurzformen fuer `Offizielle App` und `Offizielle Erweiterung`.
- `*` markiert eine quellengestuetzte Inferenz statt einer direkten Produktdokumentation. Aktuell betrifft das `Forgejo`: Codeberg ist Forgejo-basiert und dokumentiert WebAuthn-2FA; zusaetzlich ist Forgejo ein Hard-Fork von Gitea.
- `Kein offizieller Nachweis gefunden` bedeutet nicht zwingend `unmoeglich`, sondern nur, dass hier bewusst nichts behauptet wird, was ich nicht sauber belegen konnte.
- `Ja` in `Passwordless` kann projektabhaengig trotzdem mit weiteren Sicherheitsabfragen kombiniert sein; das ist in den verlinkten Quellen bzw. Issues zu pruefen.
- Die Sprachspalte ist eine grobe Einordnung der Hauptsprache des Projekts.

## Offene und negative Faelle

- `MyBB` dokumentiert offiziell `Two-Factor Authentication` mit `Authenticator Apps` und QR-Code-Setup fuer Administratoren im Admin-CP. Die allgemeine Security-Doku erwaehnt zwar `U2F` als bevorzugten Faktor-Typ, aber einen belastbaren offiziellen WebAuthn-Nachweis fuer MyBB selbst habe ich weiterhin nicht gefunden: https://docs.mybb.com/1.8/administration/security/2fa/ und https://docs.mybb.com/1.8/administration/security/protection/
- `phpBB` zeigt in den offiziellen Repositories und Erweiterungsquellen fuer mich weiter keinen belastbaren WebAuthn-Nachweis. In der deutschsprachigen Diskussion taucht nur eine Erweiterung mit `U2F` und `OTP` auf: https://www.phpbb.de/community/viewtopic.php?t=246177 und https://github.com/phpbb-extensions

## Lizenz

Die Inhalte dieses Repos stehen unter `Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)`.

- Lizenztext: [LICENSE.md](LICENSE.md)
- Offizielle Lizenz: https://creativecommons.org/licenses/by-sa/4.0/

---

Hinweis: Diese Markdown-Datei wurde mit Unterstuetzung von KI erstellt und anschliessend anhand der verlinkten Quellen strukturiert. Sofern nicht anders angegeben, stehen die Texte und Listen in diesem Repo unter CC BY-SA 4.0. Fehler, veraltete Angaben oder fehlende Projekte bitte per Issue oder Pull Request melden.
