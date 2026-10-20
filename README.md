# StickerTLWS

Transfira figurinhas do Telegram para o WhatsApp ou crie seus próprios pacotes a partir de imagens e GIFs da galeria.

[![GitHub Release](https://img.shields.io/github/v/release/Oyukihiro/StickerTLWS?style=for-the-badge&color=blue)](https://github.com/Oyukihiro/StickerTLWS/releases)

O StickerTLWS é um aplicativo Android para selecionar, editar e converter stickers e GIFs em pacotes compatíveis com o WhatsApp.

## Recursos

- **Packs do Telegram:** conecte sua conta e navegue pelos packs instalados, com stickers estáticos, animados e em vídeo.
- **Várias contas:** adicione contas Telegram e alterne entre elas mantendo sessões e catálogos separados.
- **Exportação em partes:** seleções grandes são divididas em pacotes compatíveis com o WhatsApp.
- **GIFs salvos:** selecione GIFs salvos no Telegram e converta-os em pacotes animados.
- **Criação pela galeria:** crie packs usando imagens ou GIFs do dispositivo.
- **Editor de stickers:** em imagens estáticas, ajuste o enquadramento, remova o fundo offline, adicione contorno ou texto e desenhe sobre a imagem.
- **Edição de GIFs:** ajuste o trecho e a velocidade da animação antes da conversão.
- **Prévia e organização:** confira o resultado, reorganize stickers, escolha a capa e edite os emojis associados.
- **Favoritos e filtros:** favorite stickers, GIFs e packs e encontre itens usando busca e filtros disponíveis.
- **Histórico:** consulte packs convertidos e recrie uma cópia quando os arquivos ainda estiverem disponíveis no dispositivo.
- **Backup e restauração:** salve packs, histórico, favoritos e preferências em um ZIP. Restaurar mescla os packs com os existentes.
- **Preferências:** escolha tema claro, escuro ou do sistema; selecione Português (Brasil), English ou o idioma do dispositivo; ajuste prévias e confirmações de exportação.
- **Atualizações:** verifique e baixe versões disponíveis na página de Releases.
- **Tutorial inicial:** acompanhe o fluxo para selecionar stickers, converter e adicioná-los ao WhatsApp.

## Requisitos

- Android 7.0 (API 24) ou superior.
- Uma conta Telegram para acessar seus packs e GIFs salvos.
- WhatsApp ou WhatsApp Business instalado para importar os pacotes.
- Conexão com a internet para autenticar no Telegram e baixar mídias necessárias.

## Instalação

1. Acesse [Releases](https://github.com/Oyukihiro/StickerTLWS/releases).
2. Baixe o APK adequado à arquitetura do seu dispositivo. Se não souber qual escolher, use o APK universal.
3. Abra o APK e, se solicitado, permita a instalação de aplicativos dessa fonte nas configurações do Android.
4. Abra o StickerTLWS e entre na sua conta Telegram.

## Como usar

### Exportar stickers do Telegram

1. Abra **Figurinhas** e escolha um pack.
2. Selecione a categoria de stickers estáticos ou animados.
3. Toque nos stickers que deseja exportar. É necessário selecionar ao menos 3 do mesmo tipo.
4. Inicie a exportação e confira a prévia do pacote.
5. Toque em **Adicionar ao WhatsApp** e confirme a importação no WhatsApp.
6. Se a seleção tiver mais de 30 stickers, adicione cada parte apresentada pelo app.

### Exportar GIFs salvos no Telegram

1. Abra **GIFs Salvos** e selecione pelo menos 3 itens.
2. Opcionalmente, edite o trecho e a velocidade de cada GIF.
3. Inicie a exportação, revise os pacotes gerados e adicione cada parte ao WhatsApp.

### Criar um pacote usando a galeria

1. Abra **Meus Pacotes** e escolha **Criar pacote da galeria**.
2. Selecione imagens estáticas ou GIFs animados. Não misture os tipos no mesmo pacote.
3. Escolha as mídias, dê um nome ao pacote e, se desejar, edite as imagens estáticas.
4. Crie o pacote e adicione as partes ao WhatsApp.

### Organizar e compartilhar um pacote criado

Em **Meus Pacotes**, abra as opções de um pacote para reorganizar os stickers, selecionar a capa, ajustar os emojis, compartilhar o pacote como ZIP ou excluí-lo.

## Limites dos pacotes

O WhatsApp aceita de **3 a 30 stickers por pacote**. O StickerTLWS divide automaticamente seleções maiores em partes; cada parte precisa ser adicionada separadamente no WhatsApp.

| Tipo de sticker | Dimensão máxima | Tamanho máximo do arquivo |
| --- | ---: | ---: |
| Estático | 512 × 512 px | 100 KB |
| Animado | 512 × 512 px | 500 KB |

Stickers animados e GIFs são convertidos para WebP animado e limitados a 10 segundos por sticker. Quando necessário, o app ajusta a conversão para atender aos limites de tamanho.

## Backup e dados

O backup inclui pacotes exportados, histórico, favoritos e preferências. A sessão e as credenciais do Telegram não são incluídas. Ao restaurar, os pacotes do backup são mesclados aos existentes.

O login usa o fluxo de autenticação do Telegram por meio da TDLib e pode solicitar o código de verificação e a senha da verificação em duas etapas. Sessões e arquivos locais ficam nos dados privados do aplicativo. Desinstalar o app ou limpar seus dados pode remover esses arquivos; faça um backup dos pacotes que deseja preservar.

## Compilar o projeto

### Requisitos de desenvolvimento

- Android Studio com suporte ao Android Gradle Plugin configurado no projeto.
- JDK 21.
- Android SDK configurado para o projeto.

### Debug

No Windows, a partir da pasta raiz:

```powershell
$env:JAVA_HOME = "C:\Program Files\Java\jdk-21"
$env:Path = "$env:JAVA_HOME\bin;$env:Path"
.\gradlew.bat :app:assembleDebug
```

Os APKs Debug são gerados em `app/build/outputs/apk/debug/`.

### Release

Configure a assinatura local em `%USERPROFILE%\.android\stickertlws-release.properties`:

```properties
storeFile=C:\\caminho\\para\\sua-keystore.jks
storePassword=sua-senha
keyAlias=seu-alias
keyPassword=sua-senha
```

Não compartilhe a keystore nem suas senhas e não as adicione ao repositório. Depois, execute:

```powershell
$env:JAVA_HOME = "C:\Program Files\Java\jdk-21"
$env:Path = "$env:JAVA_HOME\bin;$env:Path"
.\gradlew.bat :app:assembleRelease
```

Os APKs Release são gerados em `app/build/outputs/apk/release/`.

## Contribuir

Sugestões e relatos de bugs são bem-vindos. Abra uma [Issue](https://github.com/Oyukihiro/StickerTLWS/issues) para discutir uma ideia ou reportar um problema. Pull Requests também são bem-vindos.

## Links

- [Baixar versões (Releases)](https://github.com/Oyukihiro/StickerTLWS/releases)
- [Reportar um problema ou sugerir uma melhoria (Issues)](https://github.com/Oyukihiro/StickerTLWS/issues)
