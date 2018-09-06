''' Metodo da Secante para encontar a raiz de uma funcao
    x= x1-f(x1)*(x1-x0)/(f(x1)-f(x0)). Entrada de dados: xo, x1,
    tolerancia,numero de iteracoes maximas e funcao
'''    
def evalFunction(f, x):
        x = eval(f)
        return x


def Secante(x0,x1,tol,N,f,tipoErro):

    print(0,x0,x1)
    fx0 = evalFunction(f, x0)
    fx1 = evalFunction(f, x1)
    i=1
    h= 0.00001   #delta x para calcular a derivada de f(x)
    c = x0
    tipoErro=tipoErro
    while i<=N:
        aux = c
        x= fx1 - (fx1-x0)*f(fx1)/(f(fx1)-f(fx0))  

        print(i,x)
        if abs(x-fx1)<tol:
            return x
        i=i + 1
        if tipoErro == 'erroAbsoluto':
                        err = (c) - (aux)

                if tipoErro == 'erroRelativo':
                        err = ((c) - (aux))/(c)
        fx0=fx1    # redefinir x0
        fx1=x     #redefinir x1

    print('o metodo fracasso depois de %d iteraciones' %N)
    
import math     
    
    # Exemplo
    
f=lambda x: x**3 + 4*x**2 - 10
x0=1
x1=2
tol=0.0001
N=20
    
x=Secante(x0,x1,tol,N,f,tipoErro)
print()
print('A solcao he: ',x)
