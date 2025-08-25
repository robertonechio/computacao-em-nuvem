# Aula 4 - Relatório

Baseado nos requisitos da empresa, a alta segurança para dados sensíveis, escala para e‑commerce em datas promocionais, redução de custos, e flexibilidade para expansão futura, a solução mais equilibrada é um modelo de **nuvem híbrida**.
## Vantagens e desafios do uso da nuvem híbrida
Utilizar uma arquitetura de **nuvem híbrida**, permite manter dados sensíveis em um ambiente fechado (nuvem privada) com controles robustos (firewalls, criptografia, IAM), enquanto aproveita serviços escaláveis da nuvem pública. Outra vantagem é a escalabilidade sob demanda, onde a empresa pode usar os serviçoes de nuvem pública durante os picos de vendas, atendendo aumentos repentinos de tráfego de forma eficiente. Permite expandir conforme necessidade, migrar cargas de trabalho conforme perfil, e já ter arquitetura preparada para expansão futura. Também facilita recuperação de desastres integrando back‑up local com cloud. Alguns dos desafios ao adotar um modelo de nuvem hibrida, os modelos de nuvem privada e nuvem pública podem ter tecnologias diferentes, dificultando a integração fluida entre elas, ocorrendo alguns problemas como latência entre sistemas, incompatibilidades de APIs, diferentes formatos de dados e protocolos de comunicação. É mais difícil controlar onde os dados estão armazenados e como são processados, o que pode violar leis como a LGPD. Cada ambiente pode ter regras diferentes de auditoria, registros e retenção de dados.

## Provedores de nuvem recomendados

### Nuvem Pública (Escalabilidade, elasticidade e serviços gerenciados)
| Provedor                        | Descrição                                                 | Destaques                                                                                                |
| ------------------------------- | --------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| **AWS (Amazon Web Services)**   | Maior provedora de nuvem pública do mundo                 | Alta escalabilidade, serviços maduros (EC2, S3, RDS), integração com ambientes híbridos via AWS Outposts |
| **Microsoft Azure**             | Nuvem da Microsoft, forte integração com sistemas Windows | Boa opção para empresas com Active Directory, Office 365; oferece Azure Arc para ambientes híbridos      |
| **Google Cloud Platform (GCP)** | Nuvem do Google com foco em dados e IA                    | Fortes serviços de Big Data, IA, e containers (GKE); suporte a nuvem híbrida via Anthos                  |

### Nuvem Privada (Controle, segurança, compliance)
| Provedor/Plataforma                 | Descrição                                                 | Destaques                                                                                  |
| ----------------------------------- | --------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| **OpenStack**                       | Plataforma open-source para construção de nuvens privadas | Muito customizável; usado por empresas que precisam de controle total sobre infraestrutura |
| **VMware vSphere/Cloud Foundation** | Plataforma de virtualização corporativa                   | Permite transformar datacenters locais em nuvens privadas compatíveis com nuvem híbrida    |
| **IBM Cloud Private**               | Solução da IBM para nuvem privada                         | Foco em segurança, compliance, e integração com IBM Cloud pública                          |

### Provedores e Plataformas para Nuvem Híbrida
| Solução               | Descrição                                                               | Destaques                                                           |
| --------------------- | ----------------------------------------------------------------------- | ------------------------------------------------------------------- |
| **IBM Cloud**         | Oferece soluções híbridas com forte suporte corporativo                 | Serviços de IA, dados e integração com mainframes e nuvens privadas |
| **Red Hat OpenShift** | Plataforma de containers e orquestração híbrida                         | Suporte multi-cloud e on-premises, integra com AWS, Azure, GCP      |
| **VMware Cloud**      | Plataforma para unificar ambientes VMware on-premises com nuvem pública | Integrado com AWS, Azure, Google Cloud                              |
| **Azure Arc**         | Plataforma da Microsoft para gerenciar recursos híbridos e multi-cloud  | Gerencia servidores, Kubernetes e serviços Azure em qualquer lugar  |
| **AWS Outposts**      | Solução da AWS para trazer serviços AWS para o ambiente local           | Permite rodar AWS on-premises com mesma interface e APIs da nuvem   |

## Tabela comparativa de modelos de nuvem

| Requisito da Empresa                            | Nuvem Pública                                                                                   | Nuvem Privada                                                       | Nuvem Híbrida (Recomendada)                                                    |
| ----------------------------------------------- | ----------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| **Segurança dos dados sensíveis**               | Boa, mas menor controle                                                                         | Excelente controle e isolamento                                     | Excelente: dados sensíveis em privada, controle total                          |
| **Escalabilidade para e‑commerce em promoções** | Altíssima elasticidade                                                                          | Limitada (depende de hardware)                                      | Alta: burst escalável para pública                                             |
| **Redução de custos**                           | Baixo CapEx e modelo pay-as-you-go, pode haver custos inesperados ([Ananim Cloud][1], [IBM][2]) | Alto investimento inicial, previsível ([Ananim Cloud][1], [IBM][3]) | Balanceado: custo previsível + economia variável ([Ananim Cloud][1], [IBM][4]) |
| **Flexibilidade e expansão futura**             | Alta flexibilidade, mas menos customizável                                                      | Alta personalização, mas limitada por escala                        | Alta: combinação ideal, adaptável e escalável                                  |
| **Complexidade de gestão**                      | Menor                                                                                           | Média (gestão interna)                                              | Maior: exige integração, visibilidade e automação                              |
| **Compliance/LGPD**                             | Pode ser desafios                                                                               | Mais fácil de alinhar                                               | Ideal: dados críticos locais, outros em pública conforme regulamento           |

[1]: https://www.ananim.com.br/post/nuvem-p%C3%BAblica-privada-ou-h%C3%ADbrida-como-escolher-o-modelo-ideal-para-seu-neg%C3%B3cio?utm_source=chatgpt.com "Nuvem Pública, Privada ou Híbrida? Como escolher o modelo ideal para seu negócio"
[2]: https://www.ibm.com/br-pt/think/topics/public-cloud-vs-private-cloud-vs-hybrid-cloud?utm_source=chatgpt.com "Nuvem pública vs. nuvem privada vs. nuvem híbrida | IBM"
[3]: https://www.ibm.com/br-pt/think/insights/private-cloud-advantages-disadvantages?utm_source=chatgpt.com "Vantagens e desvantagens da nuvem privada | IBM"
[4]: https://www.ibm.com/br-pt/think/insights/hybrid-cloud-advantages-disadvantages?utm_source=chatgpt.com "Vantagens e desvantagens da nuvem híbrida | IBM"
