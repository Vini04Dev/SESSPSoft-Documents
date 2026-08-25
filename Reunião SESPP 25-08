------

## Reunião inicial 25/08 SESPP 
 
## 1. Contexto e objetivo
 
A Secretaria (SESPP) mantém hoje o programa de **Auxílio Atleta**, disponibilizado por meio de formulários no site da Secretaria. O processo atual é predominantemente manual: o participante preenche formulários, reúne a documentação exigida e envia o material, sendo toda a comunicação conduzida **por e-mail**.
 
O objetivo do projeto é construir um **sistema de gestão das solicitações de auxílio**, capaz de:
 
- centralizar a inscrição e o envio de documentos em um único fluxo;
- **gerar automaticamente os documentos oficiais** a partir dos dados informados, respeitando os modelos definidos pela Secretaria;
- **unificar toda a documentação em um único arquivo**, nomeado conforme o padrão estabelecido;
- organizar a documentação de forma que possa ser **encaminhada posteriormente à Prefeitura**;
- reduzir o tempo de tramitação, hoje estimado em **45 dias**, majoritariamente consumido pelo período de análise documental.
---
 
## 2. Base legal
 
- **Lei Municipal nº 4817, de 23/09/2021**
- **Projeto de Lei nº 5219**
> Toda regra de negócio implementada no sistema deve ser rastreável a esta legislação. Recomenda-se anexar o texto legal ao repositório do projeto como referência normativa.
 
---
 
## 3. Documentação exigida do participante
 
### 3.1 Formulários e termos
 
Documentos que hoje existem em modelo próprio e que deverão ser **gerados pelo sistema dentro do modelo oficial**, com os dados preenchidos automaticamente:
 
| Documento | Aplicação |
|---|---|
| Requerimento  modalidade individual | Participantes que competem individualmente |
| Requerimento  modalidade equipe | Participantes vinculados a equipe |
| Termo de compromisso e autorização | Todos os participantes |
| Termo de autorização dos pais | Participantes menores de 18 anos |
 
**Regra central levantada:** o documento final precisa estar **dentro do modelo oficial**, mas os **dados podem ser extraídos e preenchidos pelo sistema**. Ou seja, o sistema não altera o layout dos documentos  apenas popula os campos.
 
### 3.2 Documentos pessoais e comprobatórios
 
- **CPF**
- **RG**
- **CNH**
- **Comprovante de participação em eventos nos últimos 12 meses**, aceito em qualquer das formas:
  - lista de participantes do evento;
  - comprovante de assinatura;
  - certificado de participação.
- **Comprovante de residência atual e de 1 ano atrás**
- **Certidão criminal**  obrigatória apenas para maiores de 18 anos
- **Dados bancários**  para depósito do recurso
### 3.3 Regras por faixa etária
 
**Menores de 18 anos**
- Toda a inscrição e os dados legais são vinculados aos **pais ou responsáveis**.
- **Exceção:** os dados de participação em eventos são do próprio participante.
**Maiores de 18 anos**
- O comprovante de residência deve estar **em nome próprio**, não dos pais.
- Mesmo residindo com os pais, é possível obter uma **declaração de residência emitida pela Prefeitura**, que supre a exigência.
- Exigência adicional de **certidão criminal**.
---
 
## 4. Organização e nomenclatura dos arquivos
 
- Todos os arquivos devem ser **unidos em um único documento**.
- O nome do arquivo final segue o padrão: **data de preenchimento + nome do participante**.
- A documentação precisa ficar organizada de modo a permitir o **envio posterior à Prefeitura**.
> Implicação técnica: o sistema precisará de um módulo de **geração e concatenação de PDFs**, com preservação da ordem dos documentos e nomenclatura padronizada.
 
---
 
## 5. Fluxo do processo e prazos
 
1. Participante realiza a inscrição e envia a documentação.
2. Secretaria realiza a **análise documental**.
3. Aprovada a solicitação, o recurso é **enviado antes da competição**.
4. Participante realiza a **prestação de contas em até 3 dias após a competição**, com as **notas fiscais**.
**Prazo global atual:** 45 dias, determinado principalmente pelo período de análise dos documentos. A redução desse prazo é um dos ganhos esperados com a automação da conferência documental.
 
---
 
## 6. Regras de concessão da verba
 
- **Teto de liberação:** até **1% da verba da Secretaria**.
- **Critério de ordem:** a verba é liberada **por ordem de entrada das pessoas no sistema**  o sistema precisa registrar e preservar essa ordem de forma auditável.
- **Critérios de desempate:**
  1. participantes de **modalidades ainda não contempladas**;
  2. participantes que **ainda não receberam o suporte**.
---
 
## 7. Prestação de contas
 
- **Obrigatória** para todos os beneficiários.
- Prazo: **até 3 dias após a competição**, acompanhada das **notas fiscais**.
- **Não realizada → devolução integral do valor recebido.**
- Situações de **completude incompleta**  prestação não realizada, mal realizada ou incompleta  precisam de tratamento específico no sistema (registro da pendência e efeito sobre solicitações futuras).
---
 
## 8. Requisitos não funcionais
 
- **Acessibilidade** foi apontada como requisito para a adesão ao sistema e deve ser considerada desde o desenvolvimento, não como ajuste posterior.
- **Proteção de dados:** o sistema tratará dados pessoais sensíveis (documentos de identificação, certidão criminal, dados bancários, dados de menores), o que exige atenção à LGPD desde o desenho da solução.
---
 
## 9. Pontos em aberto  questões para a próxima reunião
 
Os itens abaixo **não estão definidos nas anotações** e precisam ser confirmados com a Secretaria antes do início da modelagem.
 
### Documentação
1. Quais documentos já presentes no formulário atual precisam ser **confirmados/validados**, e por qual critério?
2. A **CNH** substitui RG e CPF ou é exigida cumulativamente?
3. Os **modelos oficiais** de cada documento podem ser fornecidos em formato editável, para servirem de base à geração automática?
4. Documentos assinados: será aceita **assinatura digital** (gov.br, por exemplo) ou é obrigatória assinatura física digitalizada?
5. O comprovante de residência de 1 ano atrás precisa ser exatamente do mês correspondente ou há tolerância?
### Verba e concessão
6. Existe **valor máximo por atleta**, ou apenas o teto global de 1%?
7. A ordem de entrada considera a **data de início da inscrição** ou a **data de conclusão com documentação completa**?
8. Como o sistema deve se comportar quando a verba se esgota  fila de espera, indeferimento automático ou reserva para o próximo ciclo?
9. Existe periodicidade de ciclo (mensal, anual) para a liberação da verba?
### Prestação de contas
10. Qual a consequência prática para quem tem prestação de contas **incompleta ou mal realizada**  bloqueio de novas solicitações, prazo para correção, devolução parcial?
11. Existe um **modelo padrão de prestação de contas**, ou apenas o envio das notas fiscais?
12. O prazo de 3 dias é contado em dias corridos ou úteis?
### Processo e integração
13. A comunicação deve **permanecer por e-mail**, migrar para notificações no sistema, ou ambos?
14. Em que **formato** a documentação precisa chegar à Prefeitura  arquivo único por participante, lote, ou integração com algum sistema existente?
15. Quem são os **perfis de usuário** do sistema (participante, analista da Secretaria, gestor, Prefeitura) e quais permissões cada um possui?
16. Qual parte da análise documental pode ser automatizada e qual permanece obrigatoriamente humana?  este ponto define diretamente a redução dos 45 dias.
### Não funcionais
17. Existe **norma de acessibilidade** exigida pelo município (eMAG, WCAG 2.1 AA) ou padrão visual/identidade da Prefeitura a seguir?
18. Onde o sistema será **hospedado** e quem ficará responsável pela manutenção após a entrega?
19. Qual a política de **retenção e descarte** dos documentos armazenados?
------
