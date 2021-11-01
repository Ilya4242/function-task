# function-task
def func(a):
b=bin(a)[2:]
n=[x for x in b]
n.insert(0,"0")
if a&2!=0:
  for i in range(2):
    popn=n.pop(len(n)-1)
    n.insert(0,popn)
 else:
  for i in range(3):
    n.pop(0)
    n.append("0")
  l="".join(n)
  l=int(l,2)
  return(l)
