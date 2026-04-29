# Atividade 1

Esta atividade divide-se em várias partes que irão gradualmente construindo uma ferramenta simples de criptoanálise. As atividades utilizarão conhecimento - e código - das anteriores.  (IMPORTANTE: não tente fazer as partes seguintes, quando disponibilizadas, sem ter completado e entendido as anteriores)

1) Ao trabalhar com cifras, é importante sempre operar sobre bytes "raw", não codificados em strings. Porém, como estes bytes são, em geral, ilegívei, usaremos hexadecimal ou Base64 para impressão somente ("pretty printing"). Abaixo temos um exemplo, uma string em Base64 que, quando decodificada e convertida para hexadecimal, dá o seguinte resultado:
Base64: `QWNvcmRhUGVkcmluaG9RdWVob2pldGVtY2FtcGVvbmF0bw==`
hexadecimal: 41636f72646150656472696e686f517565686f6a6574656d63616d70656f6e61746f

Mas lembre-se, todas as operações sobre esta string devem usar os valores não codificados (use vetores char ou int).
Nesta primeira parte, faça funções para codificar/decodificar entre "raw", Base64 e hexadecimal.

2) Faça uma função que recebe dois buffers raw de mesmo tamanho e realiza uma cifra simples do tipo XOR. Por exemplo, fazendo XOR bit-a-bit do plaintext abaixo com a chave, obtem-se o ciphertext a seguir (em representação hexadecimal).
plaintext : 41636f72646150656472696e686f517565686f6a6574656d63616d70656f6e61746f
chave     : 0b021e0701003e0a0d060c0807063d1a0b0f0e060a1a020c0f0e03170403010f130e
ciphertext: 4a61717565616e6f697465666f696c6f6e67616c6f6e67616c6f6e67616c6f6e6761

OBS: trabalho individual ou em grupos (até 3 pessoas)

OBS 2: seu programa será testado em ambiente Linux com compilador gcc com parâmetros "-ansi -Wall"