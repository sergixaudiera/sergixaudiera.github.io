---
layout: post
title: Mapes amb R
date: 2013-01-17 15:54
categories: [personal]
---

Des de fa unes setmanesestic experimentant amb R. Un llenguatge de programació open source, pensat per fer càlculs estadístics i visualitzar-ne els resultats.

El que més m'agrada d'R, és la gran comunitat de desenvolupadors que en forma part. Aquests desenvolupadors són els que creen les llibraries  que ens serviran per calcular i representar tot el que necessitem.

En aquest exemple he utiltizat les llibraries:

- <a title="rworldmap" href="http://cran.r-project.org/web/packages/rworldmap/index.html">rworldmap</a> que de manera senzilla genera mapes del món i de diferents regions.

- <a title="classint" href="http://cran.r-project.org/web/packages/classInt/index.html" >classInt</a> pels calculs en la distribució dels països en funció del PIB he utilitzat la llibreria.

- <a title="RColorBrewer" href="http://cran.r-project.org/web/packages/RColorBrewer/index.html" >RColorBrewer</a> per l'escala de colors assignats en funció del PIB.

En aquests mapamundis comparem el PIB (GPD en anglès) en $ per a cada país del món pels anys 1990 i 2010. Aquesta comparativa ens permet observar a primer cop d'ull l'evolució del PIB per països durant 20 anys.

A continuació hi ha el codi que he empleat per crear la peça gràfica que acompanya aquesta entrada.

	#########################################
	#
	# GDP worldmap
	#
	#########################################

	data rm(UNdata_Export_20130115_054213121)

	#Renaming columns
	names(data)[1] &lt;- "ISO3V10"
	names(data)[2] &lt;- "Country"
	names(data)[3] &lt;- "nou"
	names(data)[5] &lt;- "dosmil"
	names(data)[7] &lt;- "dosmildeu"

	#Deleting columns
	data

	#Na values to 0
	data[is.na(data)]

	#Doing some maths
	data$dif10mil data$dif10nou

	#data #data

	#########################################
	#
	#Drawing colormaps with rworldwap, classint, rcolorbrewer
	#
	#########################################

	#Loading rworldmap
	library(rworldmap)

	#Joining data to a country map
	sPDF

	#Displaying a countries map
	par(mai=c(0,0,0.2,0),xaxs="i",yaxs="i")
	mapParams

	#Adding legend manually
	do.call( addMapLegend, c(mapParams, legendWidth=0.5, legendMar = 2))
	par(mai=c(0,0,0.2,0),xaxs="i",yaxs="i")

	#########################################
	#
	#Customize with ClassInt &amp; RColorBrewer
	#
	#########################################

	#Loading ClassInt, RColorBrewer
	library(classInt)
	library(RColorBrewer)

	#Getting example data and joining to a map
	data("countryExData",envir=environment(),package="rworldmap")
	sPDF , joinCode = "ISO3"
	, nameJoinColumn = "ISO3V10"
	, mapResolution='coarse'
	)

	#Getting class intervals using a 'jenks'classification in classInt package
	classInt catMethod = classInt[["brks"]]

	#Getting a colour scheme from the RColorBrewer package
	colourPalette

	#Calling mapCountryData with the parameters from classInt and RColorBrewer
	mapParams , nameColumnToPlot="dosmildeu"
	, addLegend=FALSE
	, catMethod = catMethod
	, colourPalette = colourPalette )
	do.call( addMapLegend
	, c( mapParams
	, legendLabels="all"
	, legendWidth=0.5
	, legendIntervals="data"
	, legendMar = 2 ) )
	
L'origen de les dades és el Banc Mundial.
