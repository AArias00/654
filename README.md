#!/usr/bin/env python
#-*- coding: utf-8 -*-


annéedépart=2016

année=input("Année recherchée : ")

joursemaineLISTE= ['Lundi', 'Mardi', 'Mercredi', 'Jeudi', 'Vendredi', 'Samedi', 'Dimanche']

nommoisLISTE =  ['Janvier', 'Février', 'Mars', 'Avril', 'Mai', 'Juin', 'Juillet','Août', 'Septembre', 'Octobre', 'Novembre', 'Décembre']
              
nbjourmoisLISTE = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]

joursemaineCOMPTEUR = 4
nommoisCOMPTEUR = 0
nbjourmoisCOMPTEUR = 0
jourannée=0

for jourannée in range (0,365) :
	
	jourannée = jourannée+1
	joursemaineCOMPTEUR = joursemaineCOMPTEUR+1
	nbjourmoisCOMPTEUR = nbjourmoisCOMPTEUR+1
	if joursemaineCOMPTEUR > 6 : joursemaineCOMPTEUR = 0
	if nbjourmoisCOMPTEUR > nbjourmoisLISTE[0] : nommoisCOMPTEUR=nommoisCOMPTEUR+1 
	if nbjourmoisCOMPTEUR > nbjourmoisLISTE[0] : nbjourmoisCOMPTEUR=1
	print (joursemaineLISTE[joursemaineCOMPTEUR], nbjourmoisCOMPTEUR, nommoisLISTE[nommoisCOMPTEUR], annéedépart)
	
	

	
	
