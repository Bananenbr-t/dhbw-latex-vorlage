# Befehlsübersicht
Eine kurze übersicht über die wichtigesten Befehle die in der Vorlage enthalten sind

### Überschriften und Gliederung

```TeX
\section{erste Gliederungsebene}
\subsection{zweite Gliederungsebene}
\subsubsection{dritte Gliederungsebene}
\subsubsection{dritte Gliederungsebene}
```

### Text Style
```TeX
\gqq{Anführungszeichen}
\textbf{Fettgedruckt}
\textit{Kursiv}		
\underline{Unterstrichen}
\\											% Manueller Zeilenumbruch
\myboxquote{Dieser Text steht in einer Box} % Für längere Zitate geeignet
```

### Refernzen und Verweise

```TeX
\label{referenzKey}     % Einen Referenzpunkt setzen
\ref{referenzKey}       % auf den referenzpunkt verweisen
\mypageref{referenzKey} % auf den referenzpunkt verweisen mit Seitenangabe
```
### Aufzählungen
Stichpunkte:
```TeX
\begin{itemize}								% Beginn einer Aufzählung
	\item erster Punkt						% Aufzählungspunkt
	\item Zweiter Punkt						% Aufzählungspunkt
\end{itemize}								% Ende der Aufzählung
```

Aufzählung:
```TeX
\begin{enumerate}								% Beginn einer Aufzählung
	\item erster Punkt						% Aufzählungspunkt
	\item Zweiter Punkt						% Aufzählungspunkt
\end{enumerate}								% Ende der Aufzählung
```

### Bilder
für genauerer erläuterung siehe hier:
```TeX
\begin{figure}[hbt]							% Beginn einer Grafik
	\centering 								% trim=left bottom right top
	\includegraphics[trim = 200mm 0mm 0mm 0mm, width=0.5\textwidth]{images/jubilaeum.jpg}
	\caption{Bild beschriftung} {\emph{\vgl[540]{BiBkey}}} % zweiter teil nicht im Verzeichnis
	\label{jubilaeum}
\end{figure}
```
### Tabelle
```TeX
\begin{table}[hbt]
\centering
\caption{Beschriftung {\emph{\vgl[540]{BiBkey}}}
\label{big5-korrelation}
	--> Tabelle einfügen. Als LaTeX tabelle oder Bild
\end{table}
```

### Glossar
```TeX
\gls{BPM} 								\\ 	% Glossar eintrag
\glspl{BPM} 							\\ 	% Plural des Glossar eintrags
\gls{ASM} 								\\ 	% Wenn Glossar eintrag erstamlig verwendet wird
\glspl{ASM} 							\\ 	% Wird die Bezeichnung ausgeschrieben, anschließend wird abgekürzt
```

### Literaturquellen

```TeX
\vgl{BiBkey} 							\\ 	% Vergleichs verweis ohne Seitenangabe
\vgl[2]{BiBkey} 						\\ 	% Vergleichs verweis mit Seitenangabe
\vgl[13,~46]{BiBkey}					\\ 	% Vergleichs verweis mit mehreren Seitenangaben
\cite{BiBkey} 							\\ 	% Directer Literatur aufruf
```
