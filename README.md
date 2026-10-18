# Painel de Assinaturas e Receitas do Xbox (2024)

## O que é este arquivo e para quem foi feito

O arquivo `dashboard_xbox.xlsx` reúne os dados de 295 assinantes do Xbox Game Pass ao longo de 2024 e transforma esses registros em uma tela única de acompanhamento financeiro e comercial. Ele foi pensado para diretores e gestores que precisam bater o olho nos números, entender de onde vem o dinheiro e decidir onde agir, sem precisar procurar fórmulas nem mexer nas linhas da base original.

O arquivo `Base.xlsx` original permaneceu intacto na pasta. Todo o trabalho foi construído na cópia `dashboard_xbox.xlsx`.

## Como as quatro abas funcionam e se conectam

A planilha foi dividida em quatro abas que seguem a ordem lógica A, B, C e D: `Assets`, `Bases`, `Cálculos` e `Dashboard`.

Na aba `Assets` fica guardado todo o material visual usado no painel. Lá estão a tabela com a paleta de cores oficial do Xbox, os tamanhos da fonte Segoe UI, os logotipos do Xbox, do EA Play e do Minecraft, além dos ícones originais da base. Se alguém quiser saber qual código de cor ou qual tamanho de letra foi aplicado em um cartão ou gráfico, basta consultar essa primeira aba.

A aba `Bases` guarda os registros brutos dos 295 clientes exatamente como vieram no arquivo original, organizados em uma tabela estruturada do Excel chamada `Tabela1`. Uma tabela estruturada é um formato do Excel que organiza os dados em colunas com nome fixo e expande sozinho quando novas linhas são coladas no final. Cada linha traz o código e o nome do assinante, o plano escolhido (`Core`, `Standard` ou `Ultimate`), a data de início em 2024, o status de renovação automática (`Yes` ou `No`), o preço da mensalidade base, o ciclo de cobrança (`Monthly`, `Quarterly` ou `Annual`), a compra ou não dos pacotes extras `EA Play Season Pass` e `Minecraft Season Pass`, o valor de cupom de desconto e o valor líquido pago no final. Na base original havia um filtro ativo escondendo parte das linhas; nesta versão, o filtro foi limpo para que todos os 295 clientes fiquem visíveis.

A aba `Cálculos` faz a ponte entre a base bruta e o painel visual. No lado esquerdo da aba estão as sete perguntas de negócio numeradas, acompanhadas de uma explicação simples do que foi somado ou contado e dos quadros com os resultados calculados por fórmulas diretas. No lado direito ficam quatro tabelas dinâmicas conectadas à `Tabela1`. Uma tabela dinâmica é um recurso do Excel que agrupa e soma grandes volumes de dados automaticamente sem precisar escrever fórmulas linha por linha, permitindo que os gráficos respondam aos cliques do usuário lá no painel.

A aba `Dashboard` é a tela final de leitura da diretoria, construída de forma limpa apenas com os indicadores, os gráficos e os seus respectivos títulos (toda a parte textual de explicação fica concentrada na aba `Cálculos`). A coluna A inteira foi pintada com o verde principal do Xbox (`#107C10`) e traz o logotipo branco da marca no topo. O painel começa na célula `C2` com o título geral, acompanhado pelo filtro visual `Subscription Type` no canto superior direito, quatro cartões de indicadores (linhas 5 e 6) e quatro gráficos distribuídos em dois pares (linhas 8 a 36). Tudo o que aparece nessa tela puxa os valores diretamente da aba `Cálculos`.

## Como usar o painel no dia a dia

Ao abrir a aba `Dashboard`, o diretor vê os números consolidados dos 295 clientes do ano de 2024. No canto superior direito (colunas M a Q, linhas 2 e 3) fica o filtro visual chamado `Subscription Type` (segmentação de dados, que funciona como um conjunto de botões clicáveis para filtrar os gráficos sem precisar abrir menus do Excel).

Para usar esse filtro, basta seguir três comandos simples:
1. Clique em `Annual` (anual), `Monthly` (mensal) ou `Quarterly` (trimestral) para que os gráficos mostrem apenas os números daquele ciclo de pagamento.
2. Segure a tecla `Ctrl` no teclado e clique em mais de um botão caso queira somar dois ciclos ao mesmo tempo.
3. Clique no ícone do funil com um "X" vermelho no canto superior direito da caixa do filtro para limpar a seleção e voltar a ver o ano inteiro.

Logo abaixo do cabeçalho ficam os quatro cartões de indicadores principais (KPIs, sigla usada para indicar os números-chave do negócio), trazendo apenas o título e o valor principal para leitura imediata:

O primeiro cartão (`Total EA Play Season Pass`, em `C5:E6`) mostra o total de vendas do pacote `EA Play Season Pass`, que somou R$ 2.940,00 (98 assinantes ativos, todos do plano `Ultimate`). Esse indicador ajuda a diretoria a manter o EA Play como atrativo exclusivo do plano mais completo.

O segundo cartão (`Total Minecraft Season Pass`, em `G5:I6`) traz o total de vendas do pacote `Minecraft Season Pass`, que arrecadou R$ 3.880,00 (194 assinantes nos planos `Standard` e `Ultimate`). Esse pacote responde por metade de todo o dinheiro líquido que entra na operação, apoiando a decisão de manter a venda combinada.

O terceiro cartão (`Vendas de Assinaturas (Subscription Sales)`, em `K5:M6`) apresenta as vendas de assinaturas base, que somam R$ 2.935,00 distribuídos entre os 295 clientes. Esse número serve de base para calibrar as metas de preço de tabela dos planos.

O quarto cartão (`Receita Líquida Total`, em `O5:Q6`) exibe a receita líquida que entrou de fato no caixa após descontar os cupons: R$ 7.633,00 (frente a R$ 9.755,00 de receita bruta e R$ 2.122,00 em descontos), ajudando a diretoria a acompanhar a margem real de lucro.

Abaixo dos cartões estão os quatro gráficos dinâmicos, cada um identificado diretamente pelo seu título:

O primeiro gráfico (`Vendas de Assinaturas (Subscription Sales) por Plano`, no alto à esquerda) é um gráfico de barras horizontais que mostra de onde vêm os R$ 2.935,00 das vendas de assinaturas base por plano, respondendo ao filtro de ciclo de cobrança. Ele apoia a decisão de concentrar o orçamento de divulgação no plano `Ultimate`, que gera metade da receita base mesmo tendo um terço dos clientes.

O segundo gráfico (`Receita Líquida Final vs. Descontos em Cupons por Plano`, no alto à direita) compara a receita líquida final com o valor concedido em cupons dentro de cada plano. Ele apoia a decisão de revisar a política de descontos do plano `Standard`, que perde 37,5% do seu faturamento bruto em cupons, além de incentivar a migração de clientes para o `Ultimate`.

O terceiro gráfico (`Evolução Mensal da Receita Líquida e Vendas Base (2024)`, embaixo à esquerda) mostra a evolução mês a mês da receita líquida e das vendas base de janeiro a dezembro de 2024. Ele apoia o planejamento de metas mensais e de fluxo de caixa ao mostrar que a operação estabilizou entre R$ 770,00 e R$ 832,00 por mês a partir de março.

O quarto gráfico (`Assinantes por Ciclo e Renovação Automática`, embaixo à direita) compara a quantidade de clientes com renovação automática ligada (`Yes`) e desligada (`No`) em cada modalidade de cobrança. Ele apoia uma ação imediata de retenção no ciclo mensal (`Monthly`), onde quase 80% dos clientes estão sem renovação automática.

## Perguntas de negócio respondidas na aba Cálculos

Todos os cálculos foram documentados na aba `Cálculos` a partir de sete perguntas diretas:

1. **Pergunta 1: Qual o total de vendas do pacote adicional EA Play Season Pass e quantos clientes o contrataram?** O pacote gerou R$ 2.940,00, contratado por 98 clientes (33,2% da base total e 100% dos clientes do plano `Ultimate`), o que equivale a 38,5% de toda a receita líquida da empresa.
2. **Pergunta 2: Qual o total de vendas do pacote adicional Minecraft Season Pass e qual a sua adesão na base?** O pacote gerou R$ 3.880,00 em 194 clientes (65,8% da base, contemplando todos os clientes dos planos `Ultimate` e `Standard`), representando 50,8% da receita líquida total.
3. **Pergunta 3: Qual o resumo financeiro completo da operação (mensalidades base, receita bruta, descontos e receita líquida)?** As mensalidades base somam R$ 2.935,00 e os pacotes extras somam R$ 6.820,00, formando uma receita bruta de R$ 9.755,00. Descontando os R$ 2.122,00 concedidos em cupons para 244 clientes (21,8% da receita bruta), sobram R$ 7.633,00 de receita líquida no caixa (ticket médio líquido de R$ 25,87 por cliente).
4. **Pergunta 4: Qual o valor de vendas de assinaturas base (Subscription Sales) por plano e por ciclo de cobrança?** Do total de R$ 2.935,00 em assinaturas base, o plano `Ultimate` responde por R$ 1.470,00 (50,1%, sendo R$ 675,00 no mensal, R$ 495,00 no trimestral e R$ 300,00 no anual), o `Standard` soma R$ 960,00 (32,7%, com R$ 450,00 no mensal, R$ 240,00 no trimestral e R$ 270,00 no anual) e o `Core` gera R$ 505,00 (17,2%, com R$ 245,00 no mensal, R$ 140,00 no trimestral e R$ 120,00 no anual). Por ciclo, o mensal arrecada R$ 1.370,00, o trimestral R$ 875,00 e o anual R$ 690,00.
5. **Pergunta 5: Qual plano gera mais receita líquida final após somar pacotes extras e descontar os cupons?** Embora os clientes estejam divididos quase em partes iguais (`Core` com 101, `Ultimate` com 98 e `Standard` com 96), o plano `Ultimate` entrega R$ 5.388,00 líquidos (70,6% de todo o caixa da empresa, perdendo R$ 982,00 em cupons). O plano `Standard` entrega R$ 1.801,00 líquidos (23,6% do caixa, porque perde R$ 1.079,00 em cupons sobre R$ 2.880,00 brutos). O plano `Core` gera R$ 444,00 líquidos (5,8% do caixa, com R$ 61,00 em cupons).
6. **Pergunta 6: Como evoluíram a aquisição de clientes, as vendas de assinaturas base e a receita líquida mês a mês em 2024?** Em janeiro (2 clientes, R$ 65,00 líquidos) e fevereiro (2 clientes, R$ 82,00 líquidos) o volume foi baixo. De março a novembro o ritmo manteve estabilidade de 30 a 31 novos assinantes por mês (1 por dia), gerando entre R$ 300,00 e R$ 315,00 mensais em assinaturas base e entre R$ 770,00 e R$ 832,00 mensais em receita líquida, com o melhor resultado em outubro (R$ 832,00 líquidos). Dezembro registra dados até o dia 16, com 16 clientes e R$ 389,00 líquidos, mantendo a mesma média diária.
7. **Pergunta 7: Onde está o maior risco de perda de clientes e receita por falta de renovação automática (Auto Renewal)?** No consolidado geral, 148 clientes têm renovação automática ativa (`Yes`, gerando R$ 3.786,00) e 147 não têm (`No`, somando R$ 3.847,00). O problema real aparece quando se separa por ciclo: no plano mensal (`Monthly`), 111 dos 139 clientes (79,9%) estão sem renovação automática, deixando R$ 2.824,00 expostos ao cancelamento todo mês. Já no trimestral (`Quarterly`), 60 de 85 clientes (70,6%) renovam automaticamente (R$ 806,00 sem renovação), e no anual (`Annual`), 60 de 71 clientes (84,5%) têm renovação ativa (apenas R$ 217,00 em risco).

## Cores, fonte e origem da paleta

Toda a planilha utiliza exclusivamente a fonte **Segoe UI**, que é a tipografia padrão da Microsoft e garante leitura limpa tanto em títulos grandes quanto em números pequenos.

A paleta de cores seguiu as diretrizes oficiais da marca Xbox consultadas no guia *Microsoft Xbox Brand Guidelines / Style Guide* (documentado nas referências *RelayTo Xbox Brand Guidelines* e *US Brand Colors*):
1. **Verde Xbox (`#107C10` / RGB 16, 124, 16):** cor principal da marca, aplicada no preenchimento inteiro da coluna A do `Dashboard`, nos cabeçalhos principais, nos valores de destaque dos cartões e nas barras principais dos gráficos.
2. **Verde Vibrante (`#22C55E` / RGB 34, 197, 94) e Verde Lima (`#9BC848` / RGB 155, 200, 72):** tons complementares mantidos na aba `Assets` e nos detalhes visuais secundários.
3. **Preto Grafite (`#101010` / RGB 16, 16, 16):** usado no título principal do painel (`C2`), nos cabeçalhos das perguntas de negócio, nos títulos dos cartões e na linha de comparação do gráfico mensal.
4. **Cinza Ardósia (`#3A3A3A` / RGB 58, 58, 58):** usado nos títulos de blocos, textos de apoio e rótulos de gráficos.
5. **Cinza Médio (`#737373` / RGB 115, 115, 115):** usado nos subtítulos explicativos de decisão e nas barras de comparação de cupons e clientes sem renovação automática.
6. **Cinza Claro (`#F3F4F6`) e Branco (`#FFFFFF`):** usados no fundo dos cartões de KPI, no cabeçalho dos blocos de gráficos e no fundo geral para garantir contraste e espaço em branco.

## Como atualizar os dados no futuro

Quando chegarem novas vendas ou os números do restante de dezembro de 2024, siga estes passos para atualizar o painel:

1. Abra o arquivo `dashboard_xbox.xlsx` e clique na aba `Bases`.
2. Role até a última linha da tabela (atualmente na linha 296) e cole ou digite os novos clientes a partir da linha 297, respeitando a mesma ordem das 13 colunas.
3. Como os dados estão formatados como Tabela do Excel (`Tabela1`), a tabela vai englobar as novas linhas automaticamente.
4. No menu superior do Excel, clique na guia **Dados** e depois no botão **Atualizar Tudo** (ou use o atalho `Ctrl + Alt + F5`). Isso atualiza de uma só vez todas as tabelas dinâmicas da aba `Cálculos` e todos os gráficos da aba `Dashboard`.
5. Caso inclua datas de anos posteriores a 2024 ou queira que os quadros de fórmulas fixas da aba `Cálculos` (colunas B a F) acompanhem um número maior de linhas além da linha 296, ajuste o intervalo final das fórmulas na aba `Cálculos` ou confira diretamente os totais nas tabelas dinâmicas das colunas H a K, que se ajustam sozinhas ao tamanho da `Tabela1`.

## Limitações e cuidados conhecidos

Na coluna `I` da aba `Bases` (`EA Play Season Pass Price`), os clientes que não compraram o pacote estão preenchidos com um traço (`-`) em texto em vez do número zero (`0`). As fórmulas de soma (`SOMA`) e as tabelas dinâmicas ignoram textos automaticamente e somam apenas os números, mas se alguém tentar fazer contas diretas de multiplicação linha por linha naquela coluna sem tratar o traço, o Excel mostrará erro de valor. Para preservar a regra de não alterar nenhum valor da base original, os traços foram mantidos como vieram.

Além disso, os quatro cartões de KPI no topo do `Dashboard` mostram sempre os totais fechados da operação em 2024 (vinculados às fórmulas das Perguntas 1, 2 e 3 da aba `Cálculos`), enquanto o filtro visual de ciclo (`Subscription Type`) atua sobre as tabelas dinâmicas e os gráficos do painel. Dessa forma, o diretor nunca perde a referência do faturamento total da empresa enquanto filtra os gráficos por ciclo mensal, trimestral ou anual.
