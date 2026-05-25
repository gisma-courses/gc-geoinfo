### Wie Voronoi-Polygone konstruiert werden

Voronoi-Polygone entstehen nicht durch eine inhaltliche Interpolation der Messwerte. Sie entstehen zuerst durch eine geometrische Abstandsregel. Jeder Ort im Untersuchungsraum wird demjenigen Punkt zugeordnet, zu dem er die geringste Distanz besitzt.

Die Grenze zwischen zwei benachbarten Punkten liegt dort, wo beide Punkte gleich weit entfernt sind. Konstruktiv entspricht diese Grenze der Mittelsenkrechten der Verbindungslinie zwischen den beiden Punkten. Werden diese Gleichabstandsgrenzen für alle benachbarten Punkte kombiniert, entsteht eine lückenlose Zerlegung des Raumes in Näherungszonen.

```{=html}
<iframe
  src="../assets/images/unit04/voronoi_konstruktion_svg_animation.html"
  width="100%"
  height="760"
  style="border:0; border-radius: 18px; overflow: hidden;"
  loading="lazy">
</iframe>
```

**Abbildung 04-01:** Konstruktion von Voronoi-Polygonen. Aus Punktstandorten entstehen über Gleichabstandsgrenzen und die Nächste-Punkt-Regel flächige Näherungszonen.

::: {.callout-note icon="false" appearance="simple"}
## Konstruktionsprinzip

Ein Voronoi-Polygon enthält alle Orte, die näher an seinem Ausgangspunkt liegen als an jedem anderen Punkt. Die Grenzen zwischen zwei Polygonen liegen deshalb auf Gleichabstandslinien: Jeder Ort auf einer solchen Grenze ist zu zwei benachbarten Punkten gleich weit entfernt.
:::
