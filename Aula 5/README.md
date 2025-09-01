# Aula 5 - Provedores de Computação em Nuvem


## Atividade 1
Podemos calcular o custo total, pelo uso de 5 meses, levando em conta as seguintes informações:
- O banco de dados tem o volume de 20GB de dados.
- O custo por cada GB são R$20 por mês.
- São realizadas 20.000 requisições por mês.
- A cada 1.000 requisições são cobrados R$10.
- Pela instância (máquina virtual) que hospeda o banco de dados, são cobrados R$150.

Como o volume de dados no banco de dados tem 20GB, multiplicamos 20 GB * R$20 por GB = R$400 por mês.<br>
O custo da máquina virtual tem o valor fixo de R$150.<br>
O custo das 20.000 requisições dão R$200.<br>
**Custo total por mês:** R$400 + R$150 + R$200 = R$750.<br>
**Custo total por 5 meses:** R$750 x 5 = R$3750.<br>

## Atividade 2
A instância adequada para a empresa é o intermediário, pois atende os requisitos mínimos solicitados. Se fosse escolhido a instância básica, não teria atendido os requisitos mínimos, e se fosse escolhido a instância avançada haveria o dobro de todos os itens da instância intermediaria, mas seu custo também seria dobrado.

Requisitos mínimos necessários:
- vCPU: 2 vCPUs. (Requisito atendido)
- RAM: 4 GB. (Requisito atendido)
- Armazenamento: 100 GB de SSD. (Requisito atendido)
- Rede: 20 Mbps. (Requisito atendido)

## Atividade 3
Podemos calcular o custo total, pelo uso de 24 meses, levando em conta as seguintes informações:

### Infraestrutura própria:

- 8 servidores.
- Cada servidor custa R$6000 reais.
- Os gastos com manutenção são de R$2.500 por mês.
  
#### Por 20 meses:
Custos de compra: R$6000 x 8 servidores = R$48.000.
Custo de manutenção: R$2.500 x 20 meses = R$50.000.
Custo total: R$48.000 + R$50.000 = R$98.000.

#### Por 24 meses:
Custos de compra: R$6000 x 8 servidores = R$48.000. (Continua o mesmo)
Custo de manutenção: R$2.500 x 24 meses = R$60.000.
Custo total: R$48.000 + R$60.000 = R$108.000.

### Provedor de nuvem:
- 8 servidores.
- Cada servidor em nuvem custa R$600 por mês.

#### Custo mensal:
8 servidores x R$600 = R$4.800 por mês.

#### Por 20 meses:
Custo total: R$4.800 x 20 meses = R$96.000.

#### Por 24 meses:
Custo total: R$4.800 x 24 meses = R$115.200.

Para o projeto considerando a duração de 24 meses, a solução mais economica seria a escolha de infraestrutura física, pois em 24 meses, a empresa terá um gasto de R$108.000, enquanto em nuvem, ela terá um gasto de R$115.200.
