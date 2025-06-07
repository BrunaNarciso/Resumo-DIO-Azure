# Resumo contendo resumos, anotações, como criar uma máquina vitual e dicas sobre seu uso.

## 📌 Conteúdo

- Passo a passo da criação da VM
- Acesso remoto via SSH
- Comandos úteis na VM
- Dicas de segurança e economia

**Passos sugeridos:**
Acesse o portal da Azure: https://portal.azure.com

--> Crie um recurso:

 Vá em “Criar um recurso” > “Máquina Virtual”.

-->Configure sua VM:

**Escolha:**

-Imagem: Ubuntu Server 22.04 LTS (ou Windows, se preferir)

-Tamanho da máquina: escolha um gratuito ou de baixo custo (como B1s para testes).

-Usuário e senha/SSH.

-Região: Brasil Sul ou mais próxima.

**Disco e rede:**

-Use disco padrão (HDD, se for só para testes).

-Deixe a rede com configurações padrão.

**Criação:**

-->Revise e clique em “Criar”.

**Acesse a máquina:**

-Use SSH no terminal (Linux/Mac) ou PuTTY (Windows).

---Exemplo de comando:

ssh seu-usuario@ip-da-vm

**Faça testes:**

---Atualize o sistema:

sudo apt update && sudo apt upgrade -y

---Instale pacotes (exemplo):

sudo apt install apache2 -y

**DICAS**

--Organize os recursos em "Resource Groups" (Grupos de Recursos): Isso facilita deletar tudo de uma vez quando não estiver mais usando.

--Use VMs com tamanho B1s (baixo custo): Elegível na camada gratuita.

--Desligue as VMs quando não estiver usando: Para não consumir créditos e evitar cobranças.

--Use o agendamento automático de desligamento: Em "Opções de Gerenciamento", ative o auto-shutdown com horário fixo.

--Abra apenas as portas necessárias: Ex: só porta 22 (SSH) no Linux ou 3389 (RDP) no Windows.
