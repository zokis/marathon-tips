Dicas para Maratonas de Programação
===================================

Sobre este documento
--------------------
Este documento foi iniciado por Denis Costa.

Para escrever este documento foi utilizado res

Dicas Gerais
------------

*   Sempre leia o problema todo e com atenção. Apesar de grande parte do texto
    do problema não ajudar na resolução de problema em si, as vezes informações
    importantes estão perdidas no meio do enunciado

*   Use a linguagem que você e seu time mais domina.

Declaração de Variáveis
-----------------------

Em C++
``````

Em Java
```````

Algoritmos e funções mais comuns
---------------------------

Números Primos
``````````````

Uma função muito comum em maratonas é uma função para verificar se um
número é primo. Alguns algoritmos como `Crivo de Eratóstenes`_ e o `Crivo
de Atkins`_, são algoritmos extremamente eficientes. Mas grande maioria
dos casos o código, em C++, a baixo responde muito rápido. ::

    bool is_prime(int n){
        if (n == 2) return true;
        if (n < 2 || n % 2 == 0) return false;
        for (int i = 3; i <= sqrt(n); i += 2){
            if (n % i == 0) return false;
        }
        return true;
    }

.. _Crivo de Atkins: https://en.wikipedia.org/wiki/Sieve_of_Atkin
.. _Crivo de Eratóstenes: https://en.wikipedia.org/wiki/Sieve_of_Eratosthenes
