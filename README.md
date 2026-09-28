📷 App Camera

Aplicativo desenvolvido em Flutter utilizando a linguagem Dart, com o objetivo de demonstrar o uso da câmera do dispositivo e a seleção de imagens armazenadas na galeria.

A aplicação permite que o usuário visualize a câmera, tire uma fotografia, visualize a imagem capturada e também escolha uma imagem diretamente da galeria do dispositivo.

🎯 Objetivo do projeto

O objetivo do projeto é desenvolver uma aplicação simples que utilize recursos de câmera e imagens disponíveis no dispositivo.

A aplicação permite:

📷 Abrir a câmera do dispositivo;
👁️ Visualizar a imagem da câmera em tempo real;
📸 Tirar uma fotografia;
🖼️ Visualizar a fotografia capturada;
🔄 Abrir novamente a câmera para tirar uma nova foto;
🗂️ Selecionar uma imagem existente na galeria.
🛠️ Tecnologias utilizadas
Flutter — framework utilizado para desenvolvimento da aplicação;
Dart — linguagem de programação;
Camera — biblioteca utilizada para acessar a câmera do dispositivo;
Image Picker — biblioteca utilizada para selecionar imagens da galeria;
Material Design — utilizado na construção da interface.
📦 Principais dependências

O projeto utiliza as seguintes bibliotecas:

dependencies:
  flutter:
    sdk: flutter
  cupertino_icons: ^1.0.8
  camera: ^0.12.1
  image_picker: ^1.2.3
Camera

A biblioteca camera permite acessar as câmeras disponíveis no dispositivo, inicializar a câmera e capturar fotografias.

Image Picker

A biblioteca image_picker permite que o usuário selecione uma imagem que já esteja armazenada na galeria do dispositivo.

📁 Estrutura principal do projeto
app_camera/
├── android/
├── ios/
├── lib/
│   └── main.dart
├── test/
│   └── widget_test.dart
├── assets/
│   └── camera.png
├── web/
├── windows/
├── pubspec.yaml
├── analysis_options.yaml
└── README.md
lib/main.dart

É o principal arquivo da aplicação. Nele estão implementadas as funções responsáveis pelo funcionamento da câmera e da galeria.

Entre as principais funções estão:

Inicialização da câmera;
Visualização da câmera;
Captura de fotografias;
Exibição da imagem capturada;
Abertura da câmera novamente;
Seleção de imagens da galeria.
pubspec.yaml

Arquivo responsável pelas configurações do projeto e pelo gerenciamento das bibliotecas utilizadas pela aplicação.

Também é nele que está registrado o recurso de imagem:

assets:
  - assets/camera.png
🔄 Funcionamento da aplicação

O funcionamento básico pode ser representado da seguinte maneira:

              Aplicativo
                  │
          ┌───────┴───────┐
          ↓               ↓
       Câmera           Galeria
          │               │
          ↓               ↓
    Tirar fotografia   Escolher imagem
          │               │
          └───────┬───────┘
                  ↓
          Imagem apresentada
             na tela
📸 Funcionamento da câmera

Ao abrir o aplicativo, a câmera disponível no dispositivo é identificada e inicializada.

Enquanto nenhuma fotografia foi tirada, a tela apresenta a imagem capturada pela câmera em tempo real.

O botão com o ícone de câmera permite tirar uma fotografia.

Depois que a fotografia é capturada, ela passa a ser apresentada na tela.

🔄 Tirar uma nova fotografia

Depois de tirar uma fotografia, o botão da câmera pode ser utilizado novamente para retornar à visualização da câmera.

Assim, o usuário pode tirar uma nova fotografia.

🖼️ Seleção pela galeria

O botão com o ícone de imagem permite abrir a galeria do dispositivo.

Ao selecionar uma imagem, ela é carregada e apresentada na tela da aplicação.

▶️ Como executar o projeto
1. Instalar o Flutter

É necessário ter o Flutter SDK instalado e configurado no computador.

2. Abrir a pasta do projeto

No terminal, entre na pasta do projeto:

cd app_camera
3. Instalar as dependências

Execute:

flutter pub get

Esse comando instala as bibliotecas necessárias para o funcionamento do projeto.

4. Verificar a configuração

Execute:

flutter doctor

Esse comando verifica se o ambiente Flutter está configurado corretamente.

5. Executar o aplicativo

Utilize:

flutter run

O aplicativo será executado no dispositivo ou emulador selecionado.

📱 Permissões

Como o aplicativo utiliza a câmera e a galeria do dispositivo, algumas permissões podem ser necessárias dependendo da plataforma utilizada.

No Android e no iOS, as configurações de acesso aos recursos do dispositivo devem estar corretamente definidas para que a câmera e a seleção de imagens funcionem.

⚠️ Observações
O funcionamento da câmera depende do dispositivo utilizado.
Emuladores podem possuir limitações relacionadas ao acesso à câmera.
O usuário precisa permitir o acesso à câmera quando solicitado.
O acesso à galeria também depende das permissões da plataforma.
A aplicação utiliza a primeira câmera disponibilizada pelo dispositivo.
🔮 Possíveis melhorias

O projeto pode receber novas funcionalidades no futuro, como:

📱 Alternar entre câmera frontal e traseira;
⚡ Ativar ou desativar o flash;
🔍 Adicionar zoom;
🔄 Girar ou editar imagens;
✂️ Recortar fotografias;
🗑️ Permitir excluir uma imagem selecionada;
💾 Salvar fotografias em um local específico;
📤 Compartilhar imagens;
📝 Adicionar informações ou textos sobre a imagem;
🎨 Melhorar o design da interface;
🖼️ Criar uma tela específica para visualizar as imagens.
📚 Objetivo acadêmico

Este projeto permite demonstrar conhecimentos relacionados a:

Desenvolvimento de aplicativos com Flutter;
Programação em Dart;
Criação de interfaces;
Utilização de bibliotecas externas;
Acesso aos recursos do dispositivo;
Utilização da câmera;
Seleção de arquivos de imagem;
Manipulação e apresentação de imagens.
👨‍💻 Informações do projeto

Nome: App Camera
Versão: 1.0.0+1
Framework: Flutter
Linguagem: Dart
Bibliotecas principais: Camera e Image Picker
Finalidade: Captura e seleção de imagens utilizando recursos do dispositivo.
