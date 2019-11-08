# Diário de bordo TCC

Fiz este blog com o intuito de utilizá-lo como diário de bordo do meu trabalho de conclusão de curso.
Aprendi esta técnica quando trabalhei no OMICS Lab em 2014 porém dessa vez apenas compartilharei meu markdown com essa cara mais bonitinha :)<br>
Como comecei em meados de Agosto, já estou bem avançado, mas vou tentar detalhar cada passagem por aqui.
Also esse também é um trabalho de uma optativa que estou fazendo.

### O tema

Estou trabalhando com a expressão gênica no cérebro autista, conversando com meu orientador eu disse que gostaria de utilizar o que aprendi na minha iniciação científica e que o trabalho fosse relacionado a bioinformática.
A princípio pensei num tema genérico(afinal meu curso já me deu dor de cabeça suficiente) entretanto meu orientador apresentou uma proposta para trabalharmos com dados públicos relacionados a expressão gênica de autistas. Ele também me incentivou a fazer um trabalho do qual eu me orgulhasse como último episódio dessa jornada tragicômica que foi minha graduação.Além disso utilizaremos técnicas de aprendizado de máquina para analisar os dados. :)

### Algumas considerações

Antes que eu comece a publicar o código que está em outro repositório(também não sei usar isso daqui muito bem, estou testando o Github Pages como forma de aprendizado).
Nada melhor do que ver o conteúdo teórico da faculdade na prática.
Vou tentar ser deixar o mais claro possível(ainda que essa não seja minha principal habilidade) e de acordo como eu me lembro.
O tema trata de algumas informações mais complexas mas prometo ser o mais simples possível.

### A Proposta
A proposta consistia em baixar dados públicos sobre a expressão gênica em pacientes autistas via *GEO Datasets*. Após isto verificaríamos a existência de outros grupos além dos abordados pelo artigo, os subgrupos. E para isso funcionar utilizaríamos aprendizado de máquina não supervisionado para criarmos esses subgrupos.
Eu também não queria deixar passar nenhum dado, descartando para deixar os plots apenas esteticamente melhores.
Então foi tomada a decisão de usarmos todos os dados e também colocar uma média para os pacientes válidos nos valores NAs(representação dos valores ausentes nos *dataframes*.

## Logo em Agosto, decidimos o tema, a abordagem e o cronograma que consistia em:

### Agosto

 - [x] Levantamento bibliográfico
 - [x] Levantamento da documentação dos softwares que serão utilizados 
 - [x] Planejamento do projeto 
 - [x] Entrega do pré-projeto

### Setembro

 - [x] Aplicar técnicas sobre os datasets
 - [x] Análise dos resultados 

### Outubro

 - [x] Aplicar técnicas sobre os datasets
 - [x] Análise dos resultados
 
### Novembro
 
 - [ ] Término do relatório científico
 - [ ] Publicação de resultados

## Técnicas utilizadas
 - Aprendizado não supervisionado
 - Técnica de *bootstrapping*
 - Análise de componentes principais(PCA)
 - *Clustering*

#### O que é aprendizado de máquina?
Aprendizado de Máquina é uma área de inteligência artificial (I.A.) cujo objetivo é o desenvolvimento de técnicas computacionais sobre o aprendizado bem como a construção de sistemas capazes de adquirir conhecimento de forma automática. Um sistema de aprendizado é um programa de computador que toma decisões baseado em experiências acumuladas através da solução bem sucedida de problemas anteriores. Os diversos sistemas de aprendizado de máquina possuem características particulares e comuns que possibilitam sua classificação quanto à linguagem de descrição, modo, paradigma e forma de aprendizado utilizado.

#### O que é aprendizado não supervisionado?
A indução é a forma de inferência lógica que permite obter conclusões genéricas sobre um conjunto particular de exemplos. Ela é caracterizada como o raciocínio que se origina em um conceito específico e o generaliza, ou seja, da parte para o todo.  Na indução, um conceito é aprendido efetuando-se inferência indutiva sobre os exemplos apresentados.  Portanto, as hipóteses geradas através da inferência indutiva podem ou não preservar a verdade.Mesmo assim, a inferência indutiva é um dos principais métodos utilizados para derivar conhecimento novo e predizer eventos futuros. Apesar da indução ser o recurso mais utilizado pelo cérebro humano para derivar conhecimento novo, ela deve ser utilizada com cautela, pois se o número de exemplos for insuficiente,ou se os exemplos não forem bem escolhidos, as hipóteses obtidas podem ser de pouco valor. O aprendizado indutivo é efetuado a partir de raciocínio sobre exemplos fornecidos por um processo externo ao sistema de aprendizado.  O aprendizado indutivo pode ser dividido em supervisionado e não-supervisionado.

#### O que é bootstrapping?
É um método de reamostragem proposto por Bradley Efron em 1979. Utiliza-se para aproximar distribuição na amostra de um levantamento estatístico. Usa-se frequentemente para aproximar o viés ou a variância de um conjunto de dados estatísticos, assim como para construir intervalos de confiança ou realizar contrastes de hipóteses sobre parâmetros de interesse. Na maior parte dos casos não pode obter-se expressões fechadas para as aproximações bootstrap e portanto é necessário obter reamostragens em um ordenador para pôr em prática o método. A enorme capacidade de cálculo dos computadores atuais facilita consideravelmente a aplicabilidade deste método tão custoso computacionalmente.

#### O que é análise dos componentes principais(PCA)?
A Análise de Componentes Principais é uma técnica estatística de aprendizado não supervisionado para explicar dados de alta dimensão usando um número menor de variáveis que são chamadas de componentes principais.

O PCA encontra instruções de variação máxima de dados.
Encontra direções mutuamente ortogonais. Mutuamente ortogonais significa que é um algoritmo global. Global significa que todas as direções, todos os novos recursos que eles encontram têm uma grande restrição global, a saber, que eles devem ser mutuamente ortogonais.

Basicamente o PCA transforma um conjunto de dados de alta dimensão em um subespaço de menor dimensão antes de executar um algoritmo de aprendizado de máquina nos dados.


No aprendizado não-supervisionado, o indutor analisa os exemplos fornecidos e tenta determinar se alguns deles podem ser agrupados de alguma maneira, formando agrupamentos ou clusters. Após a determinação dos agrupamentos, normalmente,é necessária uma análise para determinar o que cada agrupamento significa no contexto do problema que está sendo analisado.


## Principais problemas
 - Em Agosto, eu não esperava ter problemas, afinal era só a parte "chata" do processo.<br>Levantamento, documentação, planejamento e a entrega. Para variar deixei tudo para última hora(meia verdade) porém consegui terminar tudo a tempo.
 - Setembro passou voando e quando me dei conta faltavam menos de 2 semanas para entrarmos em Outubro. Comecei a procurar tudo o que já tinha feito anteriormente relacionado a bioinformática. Como faria a aquisição de dados, quais pacotes utilizaria, quais gráficos utilizar, como fazer funcionar aquela parte específica do código, que parâmetros usar. Durante Setembro também me surgiu uma duvida de como utilizar o aprendizado não supervisionado, eu nunca havia trabalhado com isso antes. Aliás era o que eu pelo menos achava.
 Pesquisando vi que já tinha feito algumas coisas no passado relacionadas a aprendizado não supervisionado. Realmente essa parte de documentar é muito importante. :D
 - Outubro começou e eu já tinha parte das minhas análises prontas, fui pedindo a ajuda de amigos e procurando soluções no Biostars e Stack Overflow(meia verdade novamente). Muitas perguntas, por que usar a função t(), dist() dentro dos plots? Usar somente plot() seria o suficiente? Será que o método que estou utilizando está correto? Será que estou enviesando os dados de alguma maneira?
 Contando com a ajuda do meu orientador e de alguns amigos que trabalharam comigo no laboratório, pude concluir que estava bem amparado.
Consegui bons resultados até então e aguardo as próximas reuniões para os próximos passos.
 O PVClust possui um erro de interpretação. O que é chamado de *p-value* não é exatamente *p-value* .
 *p-value* seria quanto mais se aproxima de zero e o mais distante de cem. No valor do *p-value* do PVClust funciona ao contrário.
 Por isso os valores gerados com pvrect são próximos de 100 ou 100.
 - Novembro já começamos com prazos apertados para entregar e definição da banca.
 O trabalho praticamente está finalizado e estamos em processo de escrita agora. :)

## PCA Plot com a média dos pacientes válidos
![pca1](/images/pca1.png)

## PCA Plot com os NAs omitidos
![pca2](/images/pca2.png)

## Clusterização feita com a função pvclust() confirmando os PCAs
![pvclust](/images/pvclust.png)

## Clusterização sem a função pvrect()
![pvclust_better](/images/pvclust_better.png)

## Clusterização apenas de um tecido - Cerebelo
![pvclust_cerebellum](/images/pvclust_cerebellum.png)

## Clusterização apenas de um tecido - Frontal
![pvclust_frontal](/images/pvclust_frontal.png)

## Clusterização apenas de um tecido - Temporal
![pvclust_temporal](/images/pvclust_temporal.png)

## Histograma do coeficiente de variação dos genes
![hist](/images/histograma_cv_with_omit_NA)
