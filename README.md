# Passo-a-passo-para-criar-uma-maquina-vitural-windows-no-portal-do-azure
Passo a passo para criar uma maquina vitural windows no portal do azure
1. Acessar o portal

Vá em: https://portal.azure.com

Faça login com sua conta da Microsoft (se não tiver, crie uma conta gratuita que dá R$ 200 de crédito por 30 dias).

2. Criar o recurso de Máquina Virtual

No canto superior esquerdo clique em “Criar um recurso”.

Escolha Máquina Virtual.

3. Configurações básicas (Aba Basics)

Aqui você define os dados principais da VM.

Subscription: escolha a assinatura (normalmente só aparece uma).

Resource group: crie um novo grupo (ex.: RG-VMWindows).

Nome da VM: coloque um nome, ex.: VM-Win10.

Region: escolha uma região próxima (ex.: Brazil South).

Image: escolha Windows 10 Pro, Windows 11, ou Windows Server 2019/2022 (o que você quiser testar).

Tamanho (Size): selecione um modelo básico, ex.: B1s (barato e suficiente para testes).

Usuário administrador: defina um nome de usuário (ex.: azureuser).

Senha: crie uma senha forte (guarde bem, será usada para login).

Inbound ports: marque Allow selected ports → escolha RDP (3389) para poder se conectar via Área de Trabalho Remota.

4. Disco (Aba Disks)

Escolha Premium SSD (mais rápido, mas caro) ou Standard SSD (bom para teste).

Para economizar no teste, escolha Standard HDD.

5. Rede (Aba Networking)

O Azure cria automaticamente uma rede virtual e um IP público.

Verifique se a porta RDP (3389) está aberta para conectar depois.

6. Revisar e criar

Clique em Review + Create.

O portal vai validar as configurações.

Se estiver tudo certo, clique em Create.

Espere 2–5 minutos até a VM ser provisionada.

7. Conectar na máquina virtual

Depois de criada, vá até o recurso da VM.

Clique em Connect → RDP.

Baixe o arquivo .rdp que o Azure gera.

Abra esse arquivo no seu computador → digite usuário e senha que você configurou.
