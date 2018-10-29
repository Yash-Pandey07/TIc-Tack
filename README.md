# Hang man
#Its a simple project which work to play hangman with friends 
from tkinter import *
from ranom import *
global rightcount
global wrongcount
global word
rightcount=0
wrongcount=0
wordlist=['tomcruise','therock','ryangossling','ryanreynolds','chrisevans','chrishemsworth','bendictcumberbatch','johnydepp','marlynmonroe']
word=random(wordlist)
hidden_word=[]
length=len(word)
for i in range(0,length):
	t='-'
	hidden_word.append(t)
print(hidden_word)
class pressbuttonevent:
	def __init__(self):
		window=Tk()
		label1=Label(window,text='Welcome To Hangman')
		label2=Label(window,text='The rules of the game are pretty simple\r You are given a word and you have to guess a letter untill you find out the whole word and WIN the game\r You are given 10 chances for guessing the answer and if you guess it wrong then YOU LOOSE')
		label3=Label(window,text='---------------------------------------------------------')
		a=Button(window,text='A',bg='black',fg='pink',command=self.processa)
		b=Button(window,text='B',bg='pink',fg='black',command=self.processb)
		c=Button(window,text='C',fg='pink',bg='black',command=self.processc)
		d=Button(window,text='D',bg='pink',fg='black',command=self.processd)
		e=Button(window,text='E',bg='black',fg='pink',command=self.processe)
		f=Button(window,text='F',bg='pink',fg='black',command=self.processf)
		g=Button(window,text='G',bg='black',fg='pink',command=self.processg)
		h=Button(window,text='H',bg='pink',fg='black',command=self.processh)
		i=Button(window,text='I',bg='black',fg='pink',command=self.processi)
		j=Button(window,text='J',bg='pink',fg='black',command=self.processj)
		k=Button(window,text='K',bg='black',fg='pink',command=self.processk)
		l=Button(window,text='L',bg='pink',fg='black',command=self.processl)
		m=Button(window,text='M',bg='black',fg='pink',command=self.processm)
		n=Button(window,text='N',bg='pink',fg='black',command=self.processn)
		o=Button(window,text='O',bg='black',fg='pink',command=self.processo)
		p=Button(window,text='P',bg='pink',fg='black',command=self.processp)
		q=Button(window,text='Q',bg='black',fg='pink',command=self.processq)
		r=Button(window,text='R',bg='pink',fg='black',command=self.processr)
		s=Button(window,text='S',bg='black',fg='pink',command=self.processs)
		t=Button(window,text='T',bg='pink',fg='black',command=self.processt)
		u=Button(window,text='U',bg='black',fg='pink',command=self.processu)
		v=Button(window,text='V',bg='pink',fg='black',command=self.processv)
		w=Button(window,text='W',bg='black',fg='pink',command=self.processw)
		x=Button(window,text='X',bg='pink',fg='black',command=self.processx)
		y=Button(window,text='Y',bg='black',fg='pink',command=self.processy)
		z=Button(window,text='Z',bg='pink',fg='black',command=self.processz)
	##############################################################################################################
		label1.pack()
		label2.pack()
		label3.pack()
		a.pack(side='left')
		b.pack(side='left')
		c.pack(side='left')
		d.pack(side='left')
		e.pack(side='left')
		f.pack(side='left')
		g.pack(side='left')
		h.pack(side='left')
		i.pack(side='left')
		j.pack(side='left')
		k.pack(side='left')
		l.pack(side='left')
		m.pack(side='left')
		n.pack(side='left')
		o.pack(side='left')
		p.pack(side='left')
		q.pack(side='left')
		r.pack(side='left')
		s.pack(side='left')
		t.pack(side='left')
		u.pack(side='left')
		v.pack(side='left')
		w.pack(side='left')
		x.pack(side='left')
		y.pack(side='left')
		z.pack(side='left')
		window.mainloop()
	###############################################################################################################
	def processa(self):
		guessed='a'
		print('you entered A')
		self.check(guessed)
	def processb(self):
		guessed='b'
		print('you entered B')
		self.check(guessed)
	def processc(self):
		guessed='c'
		print('you entered C')
		self.check(guessed)
	def processd(self):
		guessed='d'
		print('you entered D')
		self.check(guessed)
	def processe(self):
		guessed='e'
		print('you entered E')
		self.check(guessed)
	def processf(self):
		guessed='f'
		print('you entered F')
		self.check(guessed)
	def processg(self):
		guessed='g'
		print('you entered G')
		self.check(guessed)
	def processh(self):
		guessed='h'
		print('you entered H')
		self.check(guessed)
	def processi(self):
		guessed='i'
		print('you entered I')
		self.check(guessed)
	def processj(self):
		guessed='j'
		print('you entered J')
		self.check(guessed)
	def processk(self):
		guessed='k'
		print('you entered K')
		self.check(guessed)
	def processl(self):
		guessed='l'
		print('you entered L')
		self.check(guessed)
	def processm(self):
		guessed='m'
		print('you entered M')
		self.check(guessed)
	def processn(self):
		guessed='n'
		print('you entered N')
		self.check(guessed)
	def processo(self):
		guessed='o'
		print('you entered O')
		self.check(guessed)
	def processp(self):
		guessed='p'
		print('you entered P')
		self.check(guessed)
	def processq(self):
		guessed='q'
		print('you entered Q')
		self.check(guessed)
	def processr(self):
		guessed='r'
		print('you entered R')
		self.check(guessed)
	def processs(self):
		guessed='s'
		print('you entered S')
		self.check(guessed)
	def processt(self):
		guessed='t'
		print('you entered T')
		self.check(guessed)
	def processu(self):
		guessed='u'
		print('you entered U')
		self.check(guessed)
	def processv(self):
		guessed='v'
		print('you entered V')
		self.check(guessed)
	def processw(self):
		guessed='w'
		print('you entered W')
		self.check(guessed)
	def processx(self):
		guessed='x'
		print('you entered X')
		self.check(guessed)
	def processy(self):
		guessed='y'
		print('you entered Y')
		self.check(guessed)
	def processz(self):
		guessed='z'
		print('you entered Z')
		self.check(guessed)
	###############################################################################################
	def check(self,guess):
		if guess not in word:
			wrongcount=wrongcount+1
			print('the letter ',guess,' is not present in the word\r')
			print('you have got ',10-wrongcount,'chances left')
		else:
			print("Good going!!You guessed it right\r")
			for i in range(0,length):
				if word[i]==guess:
					hidden_word[i]=guess
					rightcount=rightcount+1
			print(hidden_word)
		if rightcount==length:
			print("Congrats you have correctly found out the word\r")
			print("the word is ",word)
		if wrongcount==1:
			print("                  * * *\r")
			print("                *  + +  *\r")
			print("                *   !   *\r")
			print("                *  ---  *\r")
			print("                  * * *\r")	
			print("                   !!!\r")
			print("          =========================\r")
			print("          =========================\r")
			print("          ==    !!!!!!!!!!!!!    ==\r")
			print("          ==    !!!!!!!!!!!!!    ==\r")
			print("          ==    !!!!!!!!!!!!!    ==\r")
			print("          ==      |==|           ==\r")
			print("                  |==| \r")
			print("                  |==| \r")
			print("                  |==| \r")
		if wrongcount==2:
			print("                  * * *\r")
			print("                *  + +  *\r")
			print("                *   !   *\r")
			print("                *  ---  *\r")
			print("                  * * *\r")
			print("                   !!!\r")
			print("          =========================\r")
			print("          =========================\r")
			print("          ==    !!!!!!!!!!!!!    ==\r")
			print("          ==    !!!!!!!!!!!!!    ==\r")
			print("          ==    !!!!!!!!!!!!!    ==\r")
			print("          ==                     ==\r")
		if wrongcount==3:
			print("                  * * *\r")
			print("                *  + +  *\r")
			print("                *   !   *\r")
			print("                *  ---  *\r")
			print("                  * * *\r")
			print("                   !!!\r")
			print("          =========================\r")
			print("          =========================\r")
			print("          ==    !!!!!!!!!!!!!    \r")
			print("          ==    !!!!!!!!!!!!!    \r")
			print("          ==    !!!!!!!!!!!!!    \r")
			print("          ==                     \r")
		if wrongcount==4:
			print("                  * * *\r")
			print("                *  + +  *\r")
			print("                *   !   *\r")
			print("                *  ---  *\r")
			print("                  * * *\r")
			print("                   !!!\r")
			print("          =========================\r")
			print("          =========================\r")
			print("                !!!!!!!!!!!!!    \r")
			print("                !!!!!!!!!!!!!    \r")
			print("                !!!!!!!!!!!!!    \r")
			print("                                 \r")
		if wrongcount==5:
			print("                  * * *\r")
			print("                *  + +  *\r")
			print("                *   !   *\r")
			print("                *  ---  *\r")
			print("                  * * *\r")
			print("                   !!!\r")
			print("          =========================\r")
			print("          =========================\r")
		if wrongcount==6:
			print("                  * * *\r")
			print("                *  + +  *\r")
			print("                *   !   *\r")
			print("                *  ---  *\r")
			print("                  * * *\r")
			print("                   !!!\r")
		if wrongcount==7:
			print("                  * * *\r")
			print("                *  + +  *\r")
			print("                *   !   *\r")
			print("                *  ---  *\r")
			print("                  * * *\r")
		if wrongcount==8:
			print("                  * * *\r")
			print("                *       *\r")
			print("                *   !   *\r")
			print("                *  ---  *\r")
			print("                  * * *\r")
		if wrongcount==9:
			print("                  * * *\r")
			print("                *       *\r")
			print("                *       *\r")
			print("                *       *\r")
			print("                  * * *\r")
		if wrongcount==10:
			print("                  \r")
			print("               \r")
			print("                \r")
			print("                \r")
			print("                  \r")

pressbuttonevent()
