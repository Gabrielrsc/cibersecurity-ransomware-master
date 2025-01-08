# Ransomware Simulado em Python

Este projeto é uma demonstração da criação de um ransomware básico utilizando a linguagem Python. Ele apresenta funcionalidades de criptografia e descriptografia de arquivos, usando o algoritmo AES no modo CTR, implementado pela biblioteca `pyaes`. Este tipo de ferramenta simula a ação de softwares maliciosos usados em ataques ransomware, onde os arquivos da vítima são criptografados e apenas restaurados mediante a uma chave específica.

## Descrição do Projeto
Este ransomware realiza as seguintes funções principais:

### Criptografia de Arquivos (encrypter)
- O script identifica um arquivo específico (ou conjunto de arquivos) no sistema para criptografia.
- Utiliza o algoritmo AES com uma chave fixa para criptografar o conteúdo dos arquivos.
- Remove o arquivo original após a criptografia, substituindo-o por um novo arquivo com a extensão modificada (`.ransomwaretroll`).

### Descriptografia de Arquivos (decrypter)
- Com a chave correta, este script reverte o processo de criptografia, restaurando o conteúdo original do arquivo.
- Lê o arquivo criptografado, descriptografa o conteúdo e recria o arquivo com o nome original, excluindo o arquivo protegido após a operação.

## Diferenciais Técnicos
### Criptografia AES em modo CTR
- **Segurança:** Este modo é reconhecido por sua segurança em aplicações que manipulam dados dinâmicos, transformando blocos de dados em fluxos de byte.
- **Simplicidade:** A implementação reúte a mesma chave para ambos os processos (criptografia e descriptografia).

### Facilidade de Implementação
- Desenvolvido em Python, o ransomware pode ser facilmente executado em vários sistemas operacionais.
- Pode operar com qualquer tipo de arquivo, desde que o nome do arquivo ou o método para identificá-lo seja fornecido.

## Aviso Importante sobre Cuidado e Ética
**Atenção**: O desenvolvimento e uso de ransomware para fins maliciosos são **ilegais** e **antiéticos**, podendo resultar em sérias consequências legais e morais. Este projeto é destinado apenas a fins educativos, como:
- Aprendizado de técnicas de criptografia.
- Desenvolvimento de soluções seguras para sistemas.
- Pesquisa e defesa contra ataques maliciosos.

Se você deseja aprimorar este projeto para torná-lo útil em aplicações de cibersegurança, estou à disposição para colaborar com melhores práticas de desenvolvimento e conformidade com padrões éticos.
