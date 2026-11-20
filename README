# Filtro de Ruído em Imagem utilizando FPGA

Projeto desenvolvido para a disciplina de **Sistemas Digitais**, da Universidade Federal de São Carlos (UFSCar), com o objetivo de implementar operações de processamento de imagens em hardware utilizando a placa FPGA DE1.

## Sobre o projeto

O projeto consiste no desenvolvimento de um sistema digital capaz de realizar o processamento de uma imagem binária com ruídos e apresentar os resultados em um monitor por meio da interface VGA.

A imagem utilizada possui resolução de **256 × 128 pixels** e é armazenada em memória ROM, permitindo a leitura dos pixels durante a execução do circuito.

A implementação foi realizada no software Quartus, utilizando diagramas de blocos (BDF) e módulos auxiliares em VHDL.

## Objetivos

- Realizar a leitura de uma imagem binária armazenada em memória;
- Implementar filtros digitais de máximo e mínimo;
- Desenvolver uma estrutura para detecção de bordas;
- Permitir a seleção dos modos de visualização por meio das chaves da FPGA;
- Exibir a imagem e os resultados do processamento em um monitor VGA.

## Tecnologias e ferramentas

- **Hardware:** FPGA DE1;
- **Software:** Quartus;
- **Linguagens:** BDF e VHDL;
- **Memória:** ROM com arquivo de inicialização MIF;
- **Interface de vídeo:** VGA.

## Estrutura do projeto

O sistema é composto por diferentes módulos que trabalham em conjunto:

| Módulo | Função |
|---|---|
| `VGA_SYNC` | Geração dos sinais de sincronização e coordenadas dos pixels |
| `video_PLL` | Geração do clock utilizado pela interface VGA |
| `rom_up` | Módulo de memória da imagem |
| `rom_mid` | Módulo de memória da imagem |
| `rom_dn` | Módulo de memória da imagem |
| `MAXN` | Operação de filtro de máximo |
| `MINV` | Operação de filtro de mínimo |
| `EDGE` | Estrutura de detecção de bordas |
| `SW0` e `SW1` | Chaves utilizadas para selecionar os modos de operação |

## Funcionamento

O funcionamento do sistema pode ser dividido nas seguintes etapas:

1. A imagem binária é armazenada em memória por meio de um arquivo MIF.
2. O circuito realiza a leitura dos pixels utilizando as coordenadas de linha e coluna.
3. Os valores dos pixels são utilizados nas operações de processamento.
4. Os circuitos de filtragem realizam operações considerando a vizinhança dos pixels.
5. As chaves `SW0` e `SW1` permitem selecionar os modos de visualização.
6. A interface VGA transmite os sinais necessários para apresentar a imagem no monitor.

A imagem é exibida na região superior esquerda da tela, enquanto a região externa à imagem permanece preta.

## Resultados

A implementação permite apresentar a imagem binária armazenada na memória diretamente no monitor conectado à FPGA DE1.

Durante os testes, foi possível visualizar as formas geométricas presentes na imagem e os pixels correspondentes aos ruídos.

## Como executar

1. Clone este repositório:

   ```bash
   git clone https://github.com/yaralima08/filtro_ruido.git
   ```

2. Abra o projeto no software Quartus.

3. Verifique se os arquivos de memória (`.mif`) e os módulos auxiliares estão disponíveis no projeto.

4. Selecione o arquivo BDF principal como entidade de topo (*Top-Level Entity*).

5. Compile o projeto.

6. Conecte a placa FPGA DE1 ao computador e programe o dispositivo utilizando o Quartus Programmer.

7. Conecte um monitor à saída VGA da placa para visualizar a imagem.

## Integrantes

- **Kailayni Rodrigues Janez** — RA 824751
- **Yara Vieira de Lima** — RA 824341

**Disciplina:** Sistemas Digitais  
**Professor:** Prof. Dr. Emerson Carlos Pedrino  
**Universidade:** Universidade Federal de São Carlos (UFSCar)  
**Ano:** 2026

## Repositório

[GitHub — Filtro de Ruído em FPGA](https://github.com/yaralima08/filtro_ruido)
