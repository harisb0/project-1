# project-1
#related to  code a game for hand cricket
print('\t\tHAND CRICKET\t\t')
print('\t\t5 OVER MATCH\t\t')
l=['ODD','EVEN']
print('1.',l[0],'\n2.',l[1])
m = input("CHOOSE : ")
if m in ('odd','ODD'):
 n = int(input('ENTER A NUMBER FOR TOSS : '))
 import random
 k = random.randrange(11)
 d = n+k
 if d%2!= 0 :
  print('you won the toss opt to : ')
  l2=['BAT','BOWL']
  print('1.',l2[0],'\n2.',l2[1])
  r=input("DECISION : ")
  if r in ('bat','BAT'):
      print("\t\tCOMPUTER READY TO BOWL\n\t\t1st INNINGS")
      sum=0
      for i in range(1,31):
       import random
       n = random.randrange(11)   
       k=int(input('BAT :'))
       print(n)
       if k == n :
        print(' BATSMEN OUT')
        print('runs scored',sum,'\nruns needed to win for the computer',sum+1)
        break
       else:
           sum=sum+k
           continue
       print('\n\t\t2nd INNINGS') 
      sum1=0
      for i in range(1,31):
       import random
       n = random.randrange(11)   
       k=int(input('BOWL :'))
       print(n)
       if k == n :
        print(' BATSMEN OUT')
        if sum1 < sum:
            print('YOU WON\nruns scored by the computer',sum1)
        print()
        break
       else:
           sum1=sum1+n
           if sum1 > sum:
               print('COMPUTER WON',sum1,'runs scored by computer')
           continue
 else  :
  print('you lost the toss ')
  l2=['BAT','BOWL']
  print(random.choice(l2))
if m in ('even','EVEN'):
 n = int(input('ENTER A NUMBER FOR TOSS : '))
 import random
 k = random.randrange(11)
 d = n+k
 if d%2 == 0 :
  print('you won the toss opt to : ')
  l2=['BAT','BOWL']
  print('1.',l2[0],'\n2.',l2[1])
 else  :
  print('you lost the toss ')
  l2=['BAT','BOWL']
  print('computer choose to',random.choice(l2))
  
  



