---
lab:
  title: 'Laboratório 3: Criar um aplicativo de tela'
  module: 'Module 3: Customize a canvas app in Power Apps'
---

# Laboratório de prática 3 – Criar um aplicativo de tela

Neste laboratório, você projetará e criará um aplicativo de tela em branco, adicionará uma fonte de dados e uma galeria.

## O que você aprenderá

- Como criar um aplicativo de tela com uma galeria vinculada a uma fonte de dados
- Como formatar campos com fórmulas do Power Fx

## Macroetapas do laboratório

- Criar um aplicativo de tela em branco
- Adicionar uma fonte de dados ao aplicativo
- Adicionar uma galeria ao aplicativo
- Configurar os campos na galeria
  
## Pré-requisitos

- Deve ter concluído o **Laboratório 2: Modelo de dados**

## Etapas detalhadas

## Exercício 1 – Criar um aplicativo de tela

### Tarefa 1.1 – Criar o aplicativo

1. Navegue até o portal do Power Apps Maker <https://make.powerapps.com>.

1. Certifique-se de que você esteja no ambiente **Dev One**.

1. Selecione a guia **+ Criar** no menu esquerdo.

1. Selecione o bloco **Aplicativo em branco** em **Iniciar de**.

    ![Captura de tela da criação em branco.](../media/create-from-blank.png)

1. Selecione **Criar** no bloco **Aplicativo de tela em branco**.

1. Insira `Booking Request app` em **Nome do aplicativo**.

1. Selecione **Tablet** em **Formato**.

    ![Captura de tela do novo nome do aplicativo.](../media/app-name-format.png)

1. Selecione **Criar**.

1. Aguarde até que o aplicativo seja criado.

1. Selecione **Salvar** no canto superior direito do Power Apps Studio.

### Tarefa 1.2 – Adicionar fonte de dados

1. No menu de criação de aplicativo, selecione **Dados**.

    ![Captura de tela do painel Dados.](../media/studio-data-pane.png)

1. Selecione o cursor suspenso ao lado de **Adicionar dados** e insira `Booking` em **Pesquisa**.

    ![Captura de tela da fonte de dados selecionada.](../media/studio-data-search.png)

1. Selecione a tabela **Solicitações de reserva** do Microsoft Dataverse.

### Tarefa 1.3 – Configurar a tela principal

1. No menu de criação do aplicativo, selecione o **Modo de exibição de árvore**.

1. Selecione **Tela1** no modo de exibição de árvore, selecione as reticências (**...**) e selecione **Renomear**.

1. Digite `MainScreen`.

1. No menu de criação do aplicativo, selecione **Inserir (+)**.

1. Selecione **Retângulo**.

1. Arraste o retângulo para o canto superior esquerdo da tela.

1. No menu de criação do aplicativo, selecione o **Modo de exibição de árvore**.

1. Renomeie o retângulo como `HeaderRect`.

1. Defina as propriedades do retângulo da seguinte maneira:

   1. X=`0`
   1. Y=`0`
   1. Altura=`80`
   1. Largura=`Parent.Width`

1. No menu de criação do aplicativo, selecione **Inserir (+)**.

1. Selecione **Rótulo de texto**.

1. Arraste o rótulo para o canto superior esquerdo da tela.

1. No menu de criação do aplicativo, selecione o **Modo de exibição de árvore**.

1. Renomeie o rótulo como `HeaderLabel`.

1. Defina as propriedades do rótulo da seguinte maneira:

   1. X=`0`
   1. Y=`0`
   1. Altura=`80`
   1. Largura=`Parent.Width`
   1. Alinhamento=`Align.Center`
   1. Tamanho=`24`
   1. Texto=`"Booking Request"`
   1. Cor=`Color.White`

    ![Captura de tela da tela principal com cabeçalho.](../media/main-screen.png)

1. Selecione **Salvar** no canto superior direito do Power Apps Studio.

### Tarefa 1.4 – Adicionar uma galeria

1. No menu de criação do aplicativo, selecione **Inserir (+)**.

1. Selecione **Galeria vertical**.

    ![Captura de tela da adição de uma galeria.](../media/add-gallery.png)

1. Selecione **Solicitações de reserva**.

    ![Captura de tela das propriedades da galeria.](../media/gallery-properties.png)

1. Selecione **Título, subtítulo e corpo** para **Layout**.

1. Selecione **7 selecionados** ao lado de **Campos**

1. Selecione **Custo** para **Corpo**.

1. Selecione **Decisão** para **Subtítulo**.

1. Selecione **Nome do animal de estimação** para **Título**.

    ![Captura de tela dos campos da galeria.](../media/select-fields.png)

1. Feche o painel Dados.

1. No menu de criação do aplicativo, selecione o **Modo de exibição de árvore**.

1. Renomeie a galeria como `BookingRequestList`.

1. Defina as propriedades da galeria da seguinte maneira:

   1. X=`0`
   1. Y=`80`
   1. Altura=`575`
   1. Largura=`250`

### Tarefa 1.5 – Formatar o campo de moeda

1. No menu de criação do aplicativo, selecione o **Modo de exibição de árvore**.

1. Expanda a galeria.

1. Selecione o corpo.

    ![Captura de tela do campo do corpo selecionado.](../media/body.png)

1. Defina a propriedade **Texto** como a fórmula:

    ```powerappsfl
    Text(Value(ThisItem.Cost), "$#,##0.00")
    ```

1. Selecione **Salvar** no canto superior direito do Power Apps Studio.

1. Selecione o botão **<- Voltar** no canto superior esquerdo da barra de comandos e selecione **Sair** para sair do aplicativo.
