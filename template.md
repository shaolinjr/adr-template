# NNNN - Nome do ADR:
NNNN é o código sequencial do ADR, que deve ser incrementado a cada novo ADR criado. 

**<ins>Exemplo</ins>**: 0001 - Utilizar ADRs para documentação

**<ins>Status</ins>**: `{Proposto | Rejeitado | Aceito | Depreciado | Substituído por }`

**<ins>Data</ins>**: `YYYY-MM-DD`

**<ins>Decisores</ins>**: [Lista de todos envolvidos na decisão]

**<ins>Consultores</ins>**: [Opcional - Lista de todos profissionais consultados durante a definição do ADR - caso tenha algum]

**<ins>Informados</ins>**: [Opcional - Lista de todos profissionais informados sobre a decisão - caso tenha alguém que não participou do ADR]

## Contexto:
Descrição do contexto/problema/situação. Deve ser direto,objetivo e conter somente as informações necessárias para a tomada de decisão, sem opiniões ou juízos de valor. Se atente ao tamanho do ADR, deve conter entre 1-2 páginas de um editor de texto padrão (ex: Word, Google Docs, etc).\
Em decisões mais complexas pode ser necessário expor mais detalhes sobre o contexto, tornando o ADR mais extenso, mas deve-se sempre levar em consideração o equilíbrio.

## Decisão:
Utilizando o formato [(WH)Y-Statements](https://www.ozimmer.ch/practices/2020/04/27/ArchitectureDecisionMaking.html) traduzido para PT-BR:

**<ins>Formato</ins>:**

**No contexto** (caso de uso, situação)\
**diante** (preocupação)\
**decidimos** (opção)\
**para alcançar** (qualidade)\
**aceitando** (desvantagem).

**<ins>Exemplo</ins>:**

**No contexto** do serviço de loja online,\
**diante** da necessidade de manter os dados de sessão do usuário consistentes e atualizados entre as instâncias da loja,\
**decidimos** pelo Padrão de Estado de Sessão em Banco de Dados e descartamos o Estado de Sessão no Cliente ou no Servidor\
**para alcançar** elasticidade na nuvem,\
**aceitando** que um banco de dados de sessão precisa ser projetado, implementado e replicado.

## Racional da Decisão:
- [Razão 1]
- [Razão 2]
- [...]

**<ins>Exemplo</ins>:**
- Manter dados de sessão do usuário consistentes e atualizados

## Opcões consideradas:
- [Opção 1]
- [Opção 2]
- [Opção 3]

**<ins>Exemplo</ins>:**
- Não utilizar sessão, usar autenticação stateless com JWT

## Consequências:
Descreva aqui o contexto resultante após a aplicação da decisão. Todas as consequências devem ser listadas, não apenas as "positivas". Seguindo o padrão:

`{Boa | Ruim}, porque {consequência}`

**<ins>Exemplos</ins>:**
- Boa, porque {consequência positiva, por exemplo, melhoria de uma ou mais qualidades desejadas, ...}
- Ruim, porque {consequência negativa, por exemplo, comprometimento de uma ou mais qualidades desejadas, ...}

## Mais informações:
Informações adicionais que possam ser relevantes para a decisão tomada, como links, referências, etc.