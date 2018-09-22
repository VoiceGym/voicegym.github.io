---
title: Konfiguration
layout: single
permalink: "/configuration/"
header:
    overlay_image: /images/configuration-splash.jpg
    overlay_filter: rgba(255, 71, 134, 0.4)
    caption: "[**Photo by Jason Olliff on Unsplash**](https://unsplash.com)"
---


<h3>Anzeige Einstellungen</h3>
<p>Hier findest du Einstellungen zur Anzeige des Spektrogramms.</p>
<div class="clearfix">
    <div class="imagediv">
    <img src="/images/screenshots/settings-view.png" alt="Settings" class="floatimage" width="40%">
    </div>

<p>Folgende Einstellungen sind möglich:</p>
<ul>
    <li>Das Frequenzband kann frei gewählt werden (von/bis Frequenz)</li>
    <li>Linear/Logarithmisch</li>
    <li>Einblenden einer Skala</li>
    <li>Anzahl der angezeigten Datenpunkte (Blöcke)</li>
</ul>

</div>

<h3>Fouriertransformations Einstellungen</h3>

<p>Mit einer größeren <b>Blockgröße</b> verbesserst du die <i>Frequenzauflösung</i> in den niedrigen Frequenzbereichen, es sinkt allerdings <i>Geschwindigkeit in der die Werte angezeigt werden</i> (schlechtere Zeitauflösung). Binning hat einen ähnlichen Effekt.</p><p> Die hier voreingestellten Werten eignen sich gut für die meisten Geräte. Jedoch um mit diese Werten zu ändern solltest zumindest das folgende verstehen.</p>

<h3>Details:</h3>
<p>Digitales Audio besteht aus einer Abfolge an Werten (Samples) die mit einer bestimmten Frequenz (Samplingfrequenz oder rate) erfasst werden. Dein Androidgerät erfasst diese Werte mit einer Frequenz von 44,1 kHz. Die Fouriertransformation benutzt eine Liste an Werten (der Block) um die Intensitäten, die in den einzelnen Frequenzen stecken, auszurechnen. Je größer der Block umso länger brauch dein Gerät um diesen zu füllen.</p>


<div class="clearfix">
    <div class="imagediv">
    <img src="/images/screenshots/settings-fourier.png" alt="Settings" class="floatimage" width="40%">
    </div>

<h3>Blockgröße:</h3>
<p>Die Anzahl an Werten in dem Datenblock die zur Fouriertransformation benutzt werden. Je größer der Block umso genauer wird die Frequenzauflösung im unteren Frequenzbereich, allerdings steigt auch die Rechenleistung deiner App.</p>

<h3>Binning:</h3>
<p>Samples werden zusammengefasst, bevor sie in den Block gefüllt werden. Ein Binning von 2 bedeutet dass 2 benachbarte Samples zu einem Wert zusammengefasst werden. Mit höherem Binning wird die Frequenzauflösung im unteren Frequenzbereich besser, jedoch sinkt die obere Frequenz für die sinnvolle Werte darstellbar sind. Für einen Binning von 2 fällt sie etwa von ca. 22 kHz auf 11 kHz. Für unsere Stimme ist jedoch der Bereich zwischen wenigen Hz bis hin zu etwa 8 kHz relevant.</p>
</div>
