# mmt_ws2223 - Shepard Effekt

---

## Konzeption Shepard-Effekt

vorgelegt von: Johnny Hänsel, Pablo Stockhausen

Für die Ausarbeitung des Shepard-Effekts werden wir unsere Konzeption in zwei Bereiche unterteilen. Zum einen die Konzeption zur Darlegung der Illusion, welche die fundamentalen Informationen zur Wirkungsweise und Funktionalität des Shepard-Effekts beinhaltet. Zum anderen die Konzept- und Planarbeit für die schrittweise Umsetzung der Audio-Illusion in der Programmiersprache Python. Darüber hinaus stellten wir fest, dass es nicht viele literarische Quellen zu diesem Thema gibt, weshalb wir eher Wissenswebseiten referenzieren werden.


#### Konzept zur Darlegung der Illusion

Das Konzept zur Darlegung der Illusion beginnt damit, dass die Grundfunktionsweise des Shepard-Effekts erläutert wird. Die Erklärung wird sich an der Definition von Roger N. Shepard orientieren, welcher den Shepard-Effekt formuliert hat. Die Konkretisierung von Besonderheiten, wie beispielsweise, dass der Shepard-Effekt jeweils mit ab- oder aufsteigenden Tönen erfolgen kann, findet zusätzlich in der allgemeinen Erklärung statt. Anschließend streben wir an, eine Unterscheidung der einzelnen Ausprägung des Shepard-Effekts darzulegen. Zu nennen ist die Shepard Skala, welche den Shepard Effekt in kurzen aufeinanderfolgenden Klängen umfasst, wobei die Frequenzveränderung in den diskreten Tonschritten erfolgt. Eine weitere Version der Skala ist die Risset-Skala oder Shepard-Risset-Glissando, indem die Teiltöne permanent gehalten und lediglich ihre Frequenzen kontinuierlich verändert werden. Darüber hinaus wird das Phänomen, dass Shepard-Töne das Tritone-Paradoxon erzeugen können beleuchtet und die Entdeckung von Pedro Praticio hinsichtlich einer Ewigen Melodie in Verbindung mit dem Shepard-Effekt aufbereitet. Anschließend werden die Faktoren und Resultate zur Wirkungsweise des Shepard Effekts auf die menschlichen Sinneseindrücke eingeordnet. Abschließend werden Zusammenhänge zu anderen Disziplinen hergestellt, wie beispielsweise, dass der Shepard Effekt auf dem gestaltpsychologischen Gesetz der Nähe basiert.

#### Konzept zur Programmierung der Illusion:

Unser Programmier-Anteil soll die Shepard-Skalar exemplarisch darstellen, bei welchem Teiltöne in aufeinander aufbauenden Frequenzen wiedergegeben werden. Zum Abspielen einzelner Töne verwenden wir die Klasse “Instrument” aus der Bibliothek “music21”. Mit dieser Bibliothek können unterschiedliche Töne und Instrumente abgespielt werden. Für eine finale Tonleiter bzw. ein finales Instrument haben wir uns noch nicht entschieden. 

Unsere Überlegung ist es, dass wir drei Tracks mit derselben Tonfolge erstellen, wobei jeder Track auf der jeweils nächsthöheren Oktave bzw. Tonhöhe beginnt. Diese können in eine hohe, mittlere und tiefe Tonlage unterschieden werden. Die Tonfolge besteht aus zwei Tonleitern mit aufbauenden Tonhöhen und umfasst somit insgesamt zwei Oktaven.

Bspw.:

- Track 1 = [C, D, E, …, c, d,e,...]

- Track 2 = [c’,d’,e’,...,c’’,d’’,e’’,...]

- Track 3 = [c’’’,d’’’,e’’’,...,e’’’’,d’’’’,e’’’’,...]

Der erste Track spielt immer leiser werdende hohe Töne. Der zweite Track spielt eine mittlere Tonhöhe, mit einer konstanten Lautstärke und der dritte Track spielt eine niedrige Tonlage, die immer lauter wird. Pro Track werden dabei mindestens 8 Töne hintereinander abgespielt, welche voraussichtlich die Tonlänge eines Halbtons haben werden, hier wollen wir jedoch mit unterschiedlichen Tonlängen experimentieren, um eine möglichst gute Illusion zu erzeugen. Zum aktuellen Zeitpunkt haben wir uns noch nicht dazu entschieden, ob die Oktave aufwärts oder abwärts abgespielt werden soll. Möglich ist es außerdem, Regler-Werte einzubauen, mit welchem die Lautstärkeentwicklung der einzelnen Oktaven angepasst werden kann. Dies würde eine experimentelle Anpassung des Programms ermöglichen, wobei gesetzte Standardwerte gewährleisten, dass die Illusion eines Shepard-Effekts dargestellt werden kann.

---