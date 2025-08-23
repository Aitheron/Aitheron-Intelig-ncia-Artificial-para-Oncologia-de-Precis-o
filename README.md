# Aitheron: Inteligência Artificial para Oncologia de Precisão

<br>


- **Nome do Estudante**: Marlon de Souza.
- **Curso**: Engenharia de Software.
- **Data de Entrega**: --

<br>

> [!NOTE]
>
> ## FAQ - Aitheron: Inteligência Artificial para Oncologia de Precisão
>
> [Informações Gerais do Projeto](https://github.com/Aitheron/Aitheron-Inteligencia-Artificial-para-Oncologia-de-Precisao/wiki)
>
> [Base de Dados e Aspectos Éticos](https://github.com/Aitheron/Aitheron-Inteligencia-Artificial-para-Oncologia-de-Precisao/wiki/Base-de-dados-e-Aspectos-%C3%89ticos-da-Pesquisa)
>
> [Entendendo o BRCA1 e BRCA2](https://github.com/Aitheron/Aitheron-Inteligencia-Artificial-para-Oncologia-de-Precisao/wiki/Entendendo-o-BRCA-e-BRCA2)
>
> [Genoma Germinativo](https://github.com/Aitheron/Aitheron-Inteligencia-Artificial-para-Oncologia-de-Precisao/wiki/Genoma-Germinativo)
>
> [Modelos de Inteligência Artificial](https://github.com/Aitheron/Aitheron-Inteligencia-Artificial-para-Oncologia-de-Precisao/wiki/Modelos-de-Intelig%C3%AAncia-Artificial)
>
> [Tipos de Mutações em BRCA1/2](https://github.com/Aitheron/Aitheron-Inteligencia-Artificial-para-Oncologia-de-Precisao/wiki/Tipos-de-Muta%C3%A7%C3%B5es-em-BRCA1-e-BRCA2)


<div align='justify'

## Resumo

&nbsp;&nbsp;&nbsp;&nbsp;Este projeto aplica técnicas de Inteligência Artificial à análise de variantes nos genes BRCA1/BRCA2 no contexto do câncer de mama. Serão desenvolvidos dois modelos de Inteligência Artificial (IA): (i) um classificador supervisionado para rotular variantes (patogênica, benigna ou de significado incerto) e (ii) um modelo probabilístico que estima o potencial patogênico de cada variante. A base de dados será consolidada a partir de ClinVar e dbSNP, normalizada para GRCh38 e enriquecida por anotações obtidas via APIs do Ensembl e por informações estruturais do UniProt, com uso de recursos como AlphaFold quando pertinente. As representações combinam atributos tabulares (coordenadas, tipo e consequência, metadados de curadoria) e informações derivadas de sequência (janelas de DNA/proteína). O segundo modelo enfatiza o impacto funcional considerando posição e transcrito afetados, tipo de evento (missense, nonsense, frameshift, alterações de splicing) e efeito esperado na proteína; eventos truncantes e alterações com perda de função tendem a elevar a probabilidade prevista. O desempenho será avaliado com métricas apropriadas e calibração de probabilidades, visando priorização interpretável de variantes e um fluxo reprodutível útil à pesquisa translacional em oncologia de precisão.

Palavras-chave: BRCA1; BRCA2; câncer de mama; variantes genéticas; inteligência artificial.

## 1. Introdução

&nbsp;&nbsp;&nbsp;&nbsp;O câncer de mama permanece um desafio relevante em saúde pública, exigindo abordagens que integrem conhecimento biológico e ferramentas computacionais. Neste contexto, propõe-se o uso de técnicas de Inteligência Artificial voltadas à análise de variantes nos genes BRCA1/BRCA2, com foco na classificação de patogenicidade e na estimativa probabilística de potencial patogênico.

&nbsp;&nbsp;&nbsp;&nbsp;A base de dados será consolidada a partir de fontes públicas como ClinVar e dbSNP, normalizada para GRCh38 e enriquecida com anotações obtidas por meio das APIs do Ensembl, além de informações estruturais provenientes de recursos como UniProt e, quando pertinente, modelos de estrutura de proteínas. As representações empregadas combinam atributos tabulares (coordenadas, tipo e consequência da variante, metadados de curadoria) e informações derivadas de sequência, de modo a capturar sinais clínicos, posicionais e biológicos relevantes.

&nbsp;&nbsp;&nbsp;&nbsp;O trabalho se organiza em dois modelos complementares. O primeiro realiza a classificação supervisionada de variantes em categorias como patogênica, benigna ou de significado incerto. O segundo estima a probabilidade de potencial patogênico considerando o contexto da mutação — posição no gene e no transcrito afetado, tipo de evento (por exemplo, missense, nonsense, frameshift ou alterações de splicing) e impacto esperado na proteína. As saídas são calibradas para produzir probabilidades interpretáveis e úteis à priorização de variantes no estudo de oncologia de precisão.

</div>

## 2. Descrição do Projeto

- **Tema do Projeto**: 

    - Oncologia: Auxiliar no tratamento do cancer de mama;
    - Proteômica: Estudo das estruturas e funções das proteínas;
    - Bioquímica Estrutural: Estrutura e funças das biomoléculas - Proteínas, aminoacidos e etc;
    - Redes Neurais Artificias: Uso de redes neurais artificiais predição de patogenicide e potencial patogênico de mutações.

<br>

- **Problemas a Resolver**: A partir de dados públicos anotados, classificar e estimar a probabilidade de patogenicidade de variantes nos genes BRCA1/BRCA2, priorizando riscos e apoiando decisões no tratamento do câncer de mama.

## 3. Referências

- [AlphaFold](https://www.youtube.com/watch?v=P_fHJIYENdI&t=1217s)
- [Dados Treinamento](http://archive.ics.uci.edu/)
- [Dados Cancer de mama](http://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic)
- [BRCA1 and BRCA2: different roles in a common pathway of genome protection](https://pmc.ncbi.nlm.nih.gov/articles/PMC4972490/)
- [Artificial intelligence-based recognition for variant pathogenicity of BRCA1 using AlphaFold2-predicted structures](https://pmc.ncbi.nlm.nih.gov/articles/PMC9800725/)
