# Aula 2 - VM do Google Cloud
Não foi possível executar tudo o que foi pedido para a aula, pois precisa ativar a API do Compute Engine no Google Cloud relacionado à faturação (billing) do projeto. Com o auxilio do ChatGPT, descobri que mesmo que eu tente acessar na forma gratuita, o Google Cloud quer garantir que existe uma forma de cobrar se o limite do uso gratuito for ultrapassado. o Compute Engine (e outros serviços da plataforma) exigem o faturamento ativado para serem usados, o erro impede a ativação da API.
## Comandos usados na aula:
```bash
gcloud config list project
export PROJECT_ID=$(gcloud config get-value project)
export REGION="us-central1"
export ZONE="us-central1-a"
echo $PROJECT_ID $REGION $ZONE
gcloud services enable compute.googleapis.com
```
## Imagens
<img width="840" height="472" alt="Captura de tela 2025-08-11 201945" src="https://github.com/user-attachments/assets/088274e2-1a21-4b31-82f3-5ec07da146df" />
<img width="840" height="472" alt="Captura de tela 2025-08-11 202109" src="https://github.com/user-attachments/assets/7e276b8e-8392-44ad-b01b-5f887b97256d" />
<img width="840" height="472" alt="Captura de tela 2025-08-11 202153" src="https://github.com/user-attachments/assets/f3a8d8e5-0e57-4849-b224-4dc9dcc150d4" />
<img width="840" height="472" alt="Captura de tela 2025-08-11 202221" src="https://github.com/user-attachments/assets/6e47e1b6-e1e4-477c-95d1-1b48ee644523" />
<img width="840" height="472" alt="Captura de tela 2025-08-11 202404" src="https://github.com/user-attachments/assets/42c91a6b-f0ba-4236-abcc-dd6bf7189fc2" />
<img width="840" height="472" alt="Captura de tela 2025-08-11 205237" src="https://github.com/user-attachments/assets/8eb9c182-7034-42df-81c1-10fb5d5bc8df" />
