# Berechnung Technischer Indikatoren

## Einfacher gleitender Durchschnitt (SMA)
Der SMA ist ein Durchschnittswert, der aus einem festgelegten Anteil der Zeitperiode berechnet wird. Die Formel für einen SMA ist:

$$ SMA = \frac{\sum_{i=1}^N Close_i}{N} $$


Der SMA ist wahrscheinlich der bekannteste Indikator in der technischen Analyse. Er wird berechnet, indem man die Schlusskurse der letzten N Perioden addiert und durch N teilt. Zum Beispiel, wenn Sie einen 20-Tage-SMA berechnen, addieren Sie die Schlusskurse der letzten 20 Tage und teilen das Ergebnis durch 20. Der SMA wird oft verwendet, um das "Rauschen" in den Preisdaten zu glätten und den zugrunde liegenden Trend besser erkennen zu können.

## Exponentieller gleitender Durchschnitt (EMA)
Der EMA ist ein gewichteter Durchschnitt, der mehr Gewicht auf die neuesten Daten legt. Die Berechnungsformel lautet:

$EMA_{heute} = (Close_{heute} \times K) + (EMA_{gestern} \times (1 - K))$

wobei $K = \frac{2}{N+1}$ der Glättungsfaktor ist.

Der EMA ist ähnlich wie der SMA, gewichtet jedoch die neueren Daten stärker als die älteren. Er wird berechnet, indem man den heutigen Schlusskurs mit einem gewissen Faktor multipliziert und den gestrigen EMA mit dem Gegenwert dieses Faktors multipliziert und dann beide Werte addiert. Der Faktor ist in der Regel $\frac{2}{N+1}$, wobei N die Länge des EMA ist.

## Relative Strength Index (RSI)
Der RSI ist ein Indikator, der das Momentum misst, indem er das Ausmaß der jüngsten Gewinne mit den jüngsten Verlusten vergleicht. Die RSI-Berechnung erfolgt in mehreren Schritten:

1. Berechnung der Aufwärts- und Abwärtsbewegungen
2. Berechnung des durchschnittlichen Gewinns und des durchschnittlichen Verlusts über N Perioden
3. Berechnung des relativen Stärke (RS), das ist das Verhältnis von durchschnittlichem Gewinn zu durchschnittlichem Verlust
4. Berechnung des RSI: 

$RSI = 100 - \frac{100}{1 + RS}$

Der RSI misst das Momentum einer Preisbewegung und bewegt sich zwischen 0 und 100. Er wird berechnet, indem man das durchschnittliche Aufwärtsmomentum über N Perioden durch das durchschnittliche Abwärtsmomentum über N Perioden teilt und das Ergebnis normiert. Ein hoher RSI (in der Regel über 70) deutet auf eine überkaufte Situation hin, während ein niedriger RSI (in der Regel unter 30) auf eine überverkaufte Situation hinweist.

## Bollinger Bänder
Bollinger Bänder sind ein Volatilitätsindikator. Sie bestehen aus einem Mittelband (ein SMA) und zwei äußeren Bändern, die jeweils einebestimmte Anzahl von Standardabweichungen vom Mittelband entfernt sind. Die Standardabweichung wird verwendet, um die Volatilität zu messen. Bollinger Bänder bestehen aus drei Linien: einem mittleren Band, das ein einfacher gleitender Durchschnitt ist, und zwei äußeren Bändern, die jeweils N Standardabweichungen vom mittleren Band entfernt sind. Sie werden verwendet, um Volatilität und mögliche überkaufte oder überverkaufte Bedingungen zu messen.

## Moving Average Convergence Divergence (MACD)
Der MACD ist ein Trendfolge-Momentum-Indikator, der die Beziehung zwischen zwei gleitenden Durchschnitten eines Wertpapiers zeigt. Der MACD wird berechnet, indem man den 26-Tage-EMA vom 12-Tage-EMA abzieht. Dieses Ergebnis ist die MACD-Linie. Dann wird ein 9-Tage-EMA der MACD-Linie berechnet und als "Signal-Linie" bezeichnet. Die Differenz zwischen der MACD-Linie und der Signal-Linie wird als Histogramm dargestellt, das als visuelle Darstellung der Divergenz/Konvergenz von MACD und Signal-Linie dient.