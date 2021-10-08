
```
FIAP
Defesa Cibernética - 1TDCF - 2021
Development e Coding for Security
Prof. MS. Fábio H. Cabrini
Atividade: Checkpoint NMAP em python
Alunos:
Laura Giancoli Aschenbrenner - RM 87194
Matheus Lambert Moreira - RM 87079
```

# PortScanner

Esse script faz scan de portas no protocolo TCP e UDP, enumerando seus respectivos serviços e salvando a saída em um arquivo .txt.

O código conta com validação das entradas, se o valor é nulo o código não é executado e o mesmo foi validado no kali linux.

Link do vídeo: https://youtu.be/F-MDA2wiDUA

## Dependências

1. python3 (sudo apt install python3 -y)
2. pip3 (sudo apt install python3-pip -y)
3. python-nmap (sudo pip3 install python-nmap) ou (sudo pip3 install python3-nmap)
4. nmap (pip3 install nmap)

## Modo de uso

```python3 script.py```

* Adicione o HOST;

* Quando solicitado, adicione a(s) porta(s) neste formato: 80 443 8080
(Com espaços como separador das portas);

* Logo em seguida, escolha o protocolo desejado.

Exemplo da saída do script:
```
#python3 script.py
Host: 127.0.0.1
Porta(s): 80 443 8080
Qual o protocolo? (Digite "UDP" ou "TCP"): TCP
Resultados no protocolo TCP para: 127.0.0.1 (127.0.0.1)
[*] tcp/80 closed http
[*] tcp/443 closed https
[*] tcp/8080 closed http-proxy

```
