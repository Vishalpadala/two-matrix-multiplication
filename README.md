# two-matrix-multiplication
A=[] m=int(input('enter number of rows:')) 
n=int(input('enter number of columns:')) 

for i in range(n):     
   row=[]     
   for j in range(n):         
     k=int(input())         
     row.append(k)     
   A.append(row) 

print(A) 

B=[] 
m=int(input('enter number of rows:'))
n=int(input('enter number of columns:')) 

for i in range(m):     
    row=[]     
    for j in range(n):         
        k=int(input())        
        row.append(k)   
    B.append(row) 

print(B)
 
C=[[0,0],[0,0]] 
for i in range(len(A)):    
    for j in range(len(B)):         
        for k in range(len(B)):             
             C[i][j]=C[i][j]+A[i][k]*B[k][j]

print('resultant matrix is:') 

for i in range(m):     
   for j in range(n):        
       print(C[i][j],end=' ')    

   print()
