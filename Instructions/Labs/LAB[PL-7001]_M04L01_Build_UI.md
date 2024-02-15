---
lab:
  title: '‘Laboratório 4: Criar a interface do usuário'
  module: 'Module 4: How to build the UI in a canvas app in Power Apps'
---

# Laboratório prático 4 – Criar a interface do usuário

Neste laboratório, você alterará as cores dos controles no aplicativo.

## O que você aprenderá

- Como usar temas
- Como personalizar seu aplicativo

## Macroetapas do laboratório

- Selecione um tema
- Personalização
  
## Pré-requisitos

- Precisa ter concluído o **Laboratório 3: Criar um aplicativo de tela**

## Etapas detalhadas

## Exercício 1 – Tema

### Tarefa 1.1 – Editar o aplicativo

1. Navegue até o portal do Power Apps Maker <https://make.powerapps.com>.

1. Certifique-se de que você esteja no ambiente **Dev One**.

1. Selecione a guia **Aplicativos** no menu esquerdo.

1. Escolha o **aplicativo Solicitação de Reserva**, selecione os Comandos (**…**) e escolha **Editar > Editar em uma nova guia**.

### Tarefa 1.2 – Selecionar um tema

1. Na barra de ações do Power Apps Studio, selecione **Tema**.

    ![Captura de tela da seleção de temas.](../media/select-theme.png)

1. Selecione o tema **Vermelho**.

### Tarefa 1.3 – Controles de marca

1. No menu de criação do aplicativo, selecione o **Modo de exibição de árvore**.

1. Expanda a galeria.

1. Selecione **NextArrow**.

1. Defina a propriedade **Color** de NextArrow para:

    ```powerappsfl
    RGBA(164, 38, 44, 1)
    ```

1. Selecione **Corpo**.

1. Defina a propriedade **Color** de Corpo para:

    ```powerappsfl
    If(ThisItem.Cost > 1000, RGBA(164, 38, 44, 1), Color.Black)
    ```

1. Selecione **Salvar** no canto superior direito do Power Apps Studio.

## Exercício 2 – Personalização

### Tarefa 2.1 – Adicionar rótulo de usuário

1. Clique fora da galeria na tela em branco.

1. No menu de criação do aplicativo, selecione **Inserir (+)**.

1. Selecione **Rótulo de texto**.

1. Arraste o rótulo para o canto superior direito da tela.

1. No menu de criação do aplicativo, selecione o **Modo de exibição de árvore**.

1. Renomeie o rótulo como `UserLabel`.

1. Defina as propriedades do rótulo da seguinte maneira:

   1. X=`1100`
   1. Y=`20`
   1. Altura=`40`
   1. Largura=`250`
   1. Alinhamento=`Align.Right`
   1. Tamanho=`18`
   1. PaddingRight=`10`
   1. Cor=`Color.White`
   1. Texto=`User().FullName`

    ![Captura de tela da tela principal com personalização.](../media/main-screen-personalized.png)

1. Selecione **Salvar** no canto superior direito do Power Apps Studio.

1. Selecione o botão **<- Voltar** no canto superior esquerdo da barra de comandos e selecione **Sair** para sair do aplicativo.
