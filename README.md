# Sistema de Gestão de Clientes

Este é um aplicativo de desktop para gerenciamento de clientes, desenvolvido em Python utilizando a biblioteca Tkinter para a interface gráfica e o módulo openpyxl para manipulação de planilhas Excel.

## Funcionalidades

- O aplicativo permite ao usuário inserir os dados de um cliente, como nome completo, contato, idade, gênero, endereço e observações.
- Os dados inseridos são salvos em uma planilha Excel chamada "Clientes.xlsx" para posterior consulta e gerenciamento.
- Caso a planilha não exista, o aplicativo cria uma nova planilha com cabeçalhos padrão para armazenar os dados.

## Como executar

Para executar o aplicativo, siga estas etapas:

1. Certifique-se de ter o Python instalado em sua máquina.
2. Instale as dependências necessárias executando o seguinte comando no terminal:
    ```
    pip install customtkinter openpyxl
3. Baixe o arquivo [app.py](app.py) para o seu ambiente de trabalho.
4. Abra um terminal na pasta onde o arquivo `app.py` está localizado.
5. Execute o seguinte comando para iniciar o aplicativo:
     ```
     python app.py
6. O aplicativo será iniciado e você verá a interface gráfica do Sistema de Gestão de Clientes.

## Como usar

1. Preencha todos os campos do formulário com as informações do cliente.
2. Clique no botão "Salvar dados" para salvar as informações do cliente na planilha.
3. Caso deseje limpar os campos do formulário, clique no botão "Limpar dados".

## Estrutura do Código

O código está organizado em uma classe chamada `App`, que herda da classe `CTk` da biblioteca CustomTkinter. Aqui está uma visão geral da estrutura do código:

- **Método `__init__`:** Inicializa a janela do aplicativo e chama os métodos `layout_config`, `appearence` e `todo_sistema`.
- **Método `layout_config`:** Configura o título e as dimensões da janela do aplicativo.
- **Método `appearence`:** Define a aparência dos elementos gráficos, como cores e temas.
- **Método `todo_sistema`:** Implementa a lógica principal do aplicativo, incluindo a criação da interface gráfica e a manipulação dos dados dos clientes.
- **Função `submit`:** Responsável por salvar os dados do cliente na planilha Excel.
- **Função `clear`:** Limpa os campos do formulário.
- **Variáveis de Texto (`name_value`, `contact_value`, `age_value`, `adress_value`):** Armazenam os valores inseridos nos campos de entrada.
- **Widgets (`name_entry`, `contact_entry`, `age_entry`, `address_entry`, `gender_combobox`, `obs_entry`, `lb_name`, `lb_contact`, `lb_age`, `lb_gender`, `lb_address`, `lb_obs`, `btn_submit`):** Elementos gráficos utilizados na interface do usuário.

## Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request com melhorias, correções de bugs ou novas funcionalidades.

- Desenvolvido por [MarcuusCorrea]
