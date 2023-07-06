# Projeto de Codificação e Decodificação Lempel-Ziv (Versão LZ78)

Este projeto implementa a codificação e decodificação do algoritmo Lempel-Ziv (Versão LZ78) usando o ambiente MARS para a linguagem de programação em assembly MIPS.

## Funcionamento do Algoritmo Lempel-Ziv (LZ78)

O algoritmo Lempel-Ziv (LZ78) é um método de compressão de dados que utiliza um dicionário para armazenar padrões encontrados no texto original. O processo de compressão é realizado da seguinte forma:

1. Inicialmente, o dicionário é criado vazio.
2. O texto original é percorrido caractere por caractere.
3. A cada novo caractere encontrado, é verificado se ele está presente no dicionário.
4. Se o caractere estiver no dicionário, ele é adicionado à sequência atual.
5. Caso contrário, a sequência atual é adicionada ao dicionário e reiniciada com o caractere atual.
6. O processo é repetido até que todo o texto original tenha sido percorrido.

Durante o processo de compressão, são gerados pares de índice e caractere, que representam as sequências encontradas no dicionário. Esses pares são armazenados no arquivo de saída codificado.

Para realizar a decodificação, o processo é inverso. O arquivo codificado é percorrido, e cada par de índice e caractere é buscado no dicionário. Os caracteres correspondentes são então adicionados à sequência final, que é gravada no arquivo de saída decodificado.

## Funcionalidades

- Codificação de um arquivo de texto utilizando o algoritmo Lempel-Ziv (Versão LZ78).
- Decodificação de um arquivo de texto codificado em formato .lzw.
- Geração de um arquivo de dicionário que permite visualizar o processo de compactação do algoritmo.

## Requisitos

- Ambiente MARS para a linguagem de programação assembly MIPS.

## Uso

1. Abra o ambiente MARS.
2. Carregue o arquivo assembly MIPS contendo a implementação do algoritmo.
3. Execute o programa.
4. O programa solicitará o caminho para o arquivo de texto de entrada.
5. Após a execução, será gerado um arquivo de texto codificado com extensão .lzw.
6. O arquivo de dicionário será gerado como resultado da codificação.
7. Para decodificar um arquivo .lzw, execute novamente o programa e escolha a opção de decodificação. Será solicitado o caminho para o arquivo .lzw a ser decodificado.
8. O arquivo de texto decodificado será gerado como resultado da decodificação.

## Documentação

A documentação do projeto inclui estatísticas de instruções utilizadas pelo programa durante a execução. Além disso, é fornecida a variação percentual dos arquivos de saída em relação ao tamanho do arquivo de entrada. Essas informações podem ser encontradas no arquivo de documentação fornecido junto com o código fonte.

## Autor

Cristóvão B. Gomes https://github.com/CristovaoBG/LWZ78MIPS

