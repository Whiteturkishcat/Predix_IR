# Predix IR — Organizador de Dados para Declaração de Imposto de Renda

Ferramenta em Excel que ajuda a reunir e organizar, de forma validada, as informações que o contribuinte vai precisar no momento de preencher a Declaração de Ajuste Anual do Imposto de Renda (IRPF). Não substitui o programa oficial da Receita Federal — o objetivo é centralizar e conferir os dados antes de declarar, reduzindo o risco de esquecer alguma informação ou informe.

Faz parte da família **Predix**, ao lado do Predix Finance (simulador de investimentos em FIIs).

## Funcionalidades (v1.0)

- **Menu de navegação lateral**, com a aba ativa destacada, para transitar entre as seções sem perder a referência visual da marca.
- **Dados do Titular**: identificação completa (nome, CPF, nascimento, título de eleitor, cônjuge, ocupação, endereço, contato), com listas suspensas validadas para os campos de resposta fechada (Sim/Não, banco, ocupação).
- **Informes de Rendimentos**: registro dos informes recebidos de cada instituição financeira, com banco selecionado por lista suspensa (evita erro de digitação e mantém o nome padronizado), valor e um campo de anexo — o usuário cola ali o hyperlink do PDF do informe correspondente, guardado em seu computador ou nuvem, para ter tudo rastreável num único lugar.
- **Notas**: registro complementar de entradas financeiras.
- **Tabelas de apoio** (abas ocultas): listas oficiais de bancos (códigos Bacen/Febraban) e de natureza de ocupação (Receita Federal), usadas como origem das listas suspensas.

## Como usar

1. Baixe o arquivo `.xlsx` deste repositório.
2. Navegue pelo menu lateral até a aba **Titular** e preencha seus dados cadastrais.
3. Na aba **Informes**, selecione o banco de cada informe recebido, informe o valor e cole o link do PDF correspondente no campo de anexo.
4. Use a aba **Notas** para registrar outras entradas relevantes.
5. Com tudo reunido e conferido, use essas informações para preencher a declaração no programa oficial da Receita Federal (ou no e-CAC).

## Estrutura do arquivo

| Aba | Conteúdo |
|---|---|
| `TITULAR` | Identificação e dados cadastrais do contribuinte |
| `INFORMES` | Informes de rendimentos por instituição financeira |
| `NOTAS` | Registro complementar de entradas |
| `Tbl_Bancos` | Tabela de apoio (oculta) — códigos e nomes das instituições financeiras |
| `Tbl_Natureza_Ocupacao` | Tabela de apoio (oculta) — códigos de natureza de ocupação da Receita Federal |

## Tecnologias

- Microsoft Excel (fórmulas nativas, validação de dados por lista)
- Tabelas de referência com base em dados oficiais (Bacen/Febraban e Receita Federal)
- Identidade visual própria (marca Predix)

## Roadmap — próxima versão (2.0)

- Detalhamento do cônjuge/companheiro (CPF, para declaração em conjunto)
- Aba de **Dependentes**, com registro individual (nome, CPF, data de nascimento, parentesco)
- Aba de **Bens e Direitos** (imóveis, veículos, contas, aplicações, criptomoedas)
- Redesenho da aba **Notas**, para registrar rendimentos sem informe formal (aluguel informal, freelance, pensão, doações)
- Classificação dos rendimentos por natureza tributária (tributável, isento, tributação exclusiva)
