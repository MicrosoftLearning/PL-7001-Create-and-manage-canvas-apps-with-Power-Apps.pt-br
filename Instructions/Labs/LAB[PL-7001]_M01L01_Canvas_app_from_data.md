---
lab:
  title: 'Laboratório 1: Criar um aplicativo de tela com base em dados'
  module: 'Module 1: Get started with Power Apps canvas apps'
---

# Laboratório de Prática 1 – Criar um aplicativo de tela com base em dados

Neste laboratório, você criará o projeto de um aplicativo de tela de uma fonte de dados existente e o compilará.

## O que você aprenderá

- Como criar aplicativos de tela do Power Apps a partir de dados e com o CoPilot
- Como se conectar ao Excel usando o OneDrive for Business como fonte de dados

## Macroetapas do laboratório

- Criar um aplicativo de tela de três telas
- Testar o aplicativo
- Criar um aplicativo de tela com o CoPilot
  
## Pré-requisitos

- Precisa ter concluído o **Laboratório 0: Validar o ambiente de laboratório**

## Etapas detalhadas

## Exercício 1 – Obter os dados

### Tarefa 1.1 – Baixar a planilha do Excel

1. Navegue até [CoffeeMachineData.xlsx](https://github.com/MicrosoftDocs/mslearn-developer-tools-power-platform/blob/master/power-apps/coffee-machine-data/CoffeeMachineData.xlsx).

1. Selecione o botão de arquivo **Raw** para baixar a pasta de trabalho do Excel.

    ![Captura de tela do ícone de download bruto no GitHub.](../media/raw-download.png)

### Tarefa 1.2 Carregar no OneDrive for Business

1. No [portal do criador do Power Apps](https://make.powerapps.com), selecione o **Inicializador de aplicativos** no canto superior esquerdo da janela do navegador e selecione o **OneDrive**.

    ![Captura de tela do ícone do OneDrive.](../media/select-onedrive.png)

1. Se for apresentada uma janela pop-up, selecione **Seu OneDrive está pronto**.

1. Selecione **+ Adicionar novo** e, em seguida, selecione **Carregar arquivos**

    ![Captura de tela do upload de arquivo do OneDrive.](../media/select-onedrive-upload.png)

1. Navegue até Downloads, selecione o arquivo CoffeeMachineData.xlsx e selecione **Abrir**.

1. Selecione **Meus arquivos** e verifique se CoffeeMachineData.xlsx foi carregado.


## Exercício 2 – Criar um aplicativo de tela de três telas

### Tarefa 2.1 – Criar o aplicativo

1. Navegue até o portal do Power Apps Maker <https://make.powerapps.com>.

1. Certifique-se de que você esteja no ambiente **Dev One**.

1. Selecione a guia **+ Criar** no menu esquerdo.

1. Selecione o bloco do **Excel** em **Iniciar de**.

    ![Captura de tela de Iniciar do Excel.](../media/start-from-excel.png)

1. Selecione **+ Nova conexão**

1. Selecione o **OneDrive for Business**, selecione **Criar**, entre com suas credenciais de locatário e selecione **Permitir acesso**.

1. Em Escolher um arquivo do Excel, localize e selecione o arquivo **CoffeeMachineData.xlsx** do Excel.

1. Em Escolher uma tabela, selecione **CoffeeMachines**.

1. Selecione **Conectar**.

1. Se a caixa de diálogo pop-up **Bem-vindo(a) ao Power Apps Studio** for exibida, selecione **Não mostrar isso novamente** e **Ignorar**.

1. Aguarde até que o aplicativo seja criado.

    ![Captura de tela da tela de Procurar na tela em um aplicativo de três telas.](../media/three-screen-app-browse-screen.png)

1. Selecione **Salvar** no canto superior direito do Power Apps Studio, insira `Coffee Machines App` e selecione **Salvar**.


### Tarefa 2.2 – Testar o aplicativo

1. Selecione o ícone de **pré-visualização do aplicativo** no canto superior direito do Power Apps Studio.

1. Selecione qualquer computador na galeria. Isso navega até a tela Detalhes,

1. Selecione o ícone **Editar** no canto superior direito do aplicativo. Isso abre a tela Editar.

1. Altere o **Preço do computador** e selecione o ícone de confirmação **Enviar item** no canto superior direito do aplicativo.

1. Selecione o ícone **<** no canto superior esquerdo do aplicativo.

1. Selecione o ícone **+** no canto superior direito do aplicativo.

1. Insira `97` em **ID do computador**.

1. Insira `Demo Machine` em **Nome do computador**.

1. Insira `999` em **Preço do computador**.

1. Selecione o ícone **Enviar item** no canto superior direito do aplicativo.

1. Insira `Demo` em **Itens de pesquisa**.

1. Selecione **X** no canto superior direito para interromper a pré-visualização.

1. Se for exibida a caixa de diálogo pop-up **Você sabia? **, selecione **Não mostrar isso novamente** e selecione **Ok**.

1. Selecione o botão **<- Voltar** no canto superior esquerdo da barra de comandos e escolha **Sair** para sair do aplicativo.


## Exercício 3 – Criar um aplicativo de tela com o Copilot

### Tarefa 3.1 – Criar o aplicativo

1. Navegue até o portal do Power Apps Maker `https://make.powerapps.com`

1. Verifique se você está no ambiente **Dev One**.

1. Selecione a guia **Página Inicial** no menu de navegação à esquerda. 

   > Se a opção **Experimentar a nova experiência do Power Apps** estiver habilitada, desative-a para que este laboratório funcione corretamente.
   > Lançaremos novos laboratórios em breve com a experiência atualizada.

1. Em **Vamos criar um aplicativo. O que ele deve fazer?** insira `Assign coffee repairs to technicians per customer request` e selecione o ícone de seta **Ir** para enviar.

    ![Captura de tela de solicitação do copilot.](../media/copilot-prompt.png)

    O Copilot começará a criar uma estrutura de tabela para dar suporte ao aplicativo.

    > **IMPORTANTE:** Ao usar a IA gerativa, nem sempre você obterá os mesmos resultados exatos. É possível que sua tabela não corresponda exatamente à tabela criada para outro aluno. 

    > Para ver a estrutura da tabela, escolha a tabela e clique no botão **Exibir dados** 
1. Examinar a tabela

    ![Captura de tela da tabela de copiloto.](../media/copilot-table.png)

1. Quando estiver contente com a tabela, clique no botão **Salvar e abrir aplicativo**. 

1. Se necessário, na tela **Concluiu o trabalho?**, clique em **Não perguntar novamente** e clique no botão **Salvar e abrir aplicativo**. 

1. Aguarde até que o aplicativo seja criado.

    ![Captura de tela do aplicativo por copiloto.](../media/copilot-app.png)

1. Selecione **Salvar** no canto superior direito do Power Apps Studio.

1. Selecione o botão **<- Voltar** no canto superior esquerdo da barra de comandos e selecione **Sair** para sair do aplicativo.

1. Selecione a guia **Aplicativos** no menu esquerdo do portal do criador do Power Apps.
