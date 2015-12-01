<h1>SEO Tool v2 by damianschwyrz.de</h1>
<p>Das Tool bietet im Grunde die gleichen Funktionen, wie die erste Version. Hinzugekommen sind einige neue Funktionen, die Codebasis wurde komplett überarbeitet. Außerdem kommt ein ordentliches Adminpanel zum Einsatz. Ich hab mich da für SB Admin entschieden.</p>
<h2>Voraussetzungen</h2>
<p>Wie auch schon bei der ersten Version: Es ist notwendig einen Cronjob per SSH auszuführen, d.h. ein normaler Webspace reicht in der Regel nicht aus. Ursächlich hierfür ist, dass das auszuführende Programm in Perl geschrieben ist und je nach Anzahl von Keywords bis zu 45 Minuten am Stück aktiv ist. So etwas lässt sich nur schwer mit PHP realisieren, man müsste in den Serverkonfigurationen einiges abändern (Max Exec Time etwa,...).</p>

<strong>Ansonsten:</strong>
<ul>
<li>Server mit SSH-Zugang (d.h. kein Webspace nicht geeignet)</li>
<li>PHP 5.6</li>
<li>MYSQL 5.5</li>
<li>PERL 5.20</li>
<li>Grundlegende Serveradmin-Kenntnisse</li>
<li>Subdomain</li>
</ul>

<h2>Installationsanleitung</h2>
<p>Ich bitte die folgende Anweisung exakt zu lesen und zu befolgen. Der Installationsprozess gestaltet sich hier nicht trifvial, wer das Tool nutzen will, aber nicht in der Lage ist es aufzusetzen, <strong>kann mich beauftragen</strong> einen kleinen Server mit dem Tool aufzusetzen. Hier reichen kleine vServer vollkommen aus.</p>

<h3>Schritt 1: Subdomain einrichten</h3>
<p>Das Tool funktioniert ausschließlich unter einer Subdomain. Legt diese mit einer eurer Domains an - eine TLD allgemein oder IP-Adresse wird ebenfalls funktionieren.</p>
<h3>Schritt 2: Repo klonen oder herunterladen</h3>
<p>Einfach alle Dateien, die man hier im Repo sieht an die entsprechende Stelle klonen bzw. das Paket herunterladen. Meist ist das sowas wie: /var/www/euredomain.de/web/</p>
<h3>Schritt 3: htaccess/nginx anpassen</h3>
<p>Das Tool wurde mit dem SLIM Framework 3 RC2 programmiert und entsprechend gilt die folgende Anleitung: Weiter zu <a href="http://www.slimframework.com/docs/start/web-servers.html" target="_blank">slimframework.com</a></p>