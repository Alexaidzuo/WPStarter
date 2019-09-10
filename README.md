# Setovanje projekta

1. Ukoliko ste uradili pripremu, potrebno je skinuti poslednju verziju WordPress-a i extract-ovati je u repository u www folderu

2. Napraviti bazu u phpmyadminu i instalirati WordPress

3. Ubaciti WPStarter temu u /wp-content/themes/

4. Promeniti naziv foldera teme iz WPStarter u naziv projekta

5. Na nivou foldera teme izvršiti globalni find/replace za slug WPStarter u svim fajlovima i zameniti ga nazivom projekta

6. Promeniti Theme Name: WP Starter u fajlu /wp-content/themes/starter_s/assets/sass/style.scss

7. Kopirati favicon i screenshot teme (dizajner priprema)

8. Unutar foldera teme uraditi npm install

9. Ukoliko je potrebno uključiti bootstrap /wp-content/themes/starter_s/assets/sass/style.scss skinuti komentar sa linije koja poziva bootstrap grid

10. U terminalu ukucati gulp build (gulp build generise dist folder sa minifikovanim javascriptom i css-om, takođe generiše fajlove style.css na osnovu koga wordpress prepoznaje temu)

11. U rootu projekta napraviti .gitignore fajl

```
wp-content/ai1wm-backups
node_modules
wp-config.php
.sass-cache
.idea
wp-content/mu-plugins/wp-migrate-db-pro-compatibility.php
wp-content/uploads/wp-migrate-db/
*.zip
```

## Napomena:
- Ukoliko ne uradite gulp build nećete moći aktivirati temu u dashboard-u, pisaće "missing stylesheet" jer nije generisan glavni *.css fajl

<hr>

1. Aktivirati temu u dashboard-u

2. Obrisati ostale teme (ako ih ima)

3. Ukloniti sve Widget-e

4. Obrisati "Hello World" post iz Posts

5. Obrisati "Sample Page" iz Pages

6. Kreirati "Homepage" stranicu i dodeliti joj template "Homepage"

7. Podesiti "Homepage" kao Front Page u Settings > Reading

8. Obrisati Tagline u Settings > General

9. Podesiti Permalinks na Post Name

10. Kreirati primarnu navigaciju

11. Instalirati/aktivirati potrebne pluginove
