# StickerTLWS

[!](https://i.ibb.co/4Rx18Yyq/ic-launcher-web.png)

## App Android para mover suas figurinhas e GIFs do Telegram diretamente para o WhatsApp com facilidade e rapidez.

## Página de Releases para baixar o APK: [clique aqui](https://github.com/Oyukihiro/StickerTLWS/releases).

[![](https://img.shields.io/github/v/release/Oyukihiro/StickerTLWS?style=for-the-badge&color=blue)](https://github.com/Oyukihiro/StickerTLWS/releases)

### Principais Funcionalidades:

- **Integração Nativa com Telegram**: Faça login com seu número e acesse todos os seus pacotes instantaneamente via TDLib.
- **Conversão Inteligente**: Converte stickers estáticos, animados (TGS) e de vídeo (WebM) para o formato compatível com o WhatsApp.
- **Suporte a GIFs**: Exporte seus GIFs salvos do Telegram como pacotes de figurinhas animadas.
- **Interface Moderna**: UI construída totalmente em Jetpack Compose com Material 3, efeitos de Glassmorphism e animações fluidas.
- **Multi-idioma**: Suporte completo para Português (Brasil) e Inglês com seletor rápido na tela inicial.
- **Gerenciamento de Pacotes**: Aba dedicada para visualizar, excluir e gerenciar os pacotes que você já criou.
- **Prévia ao Pressionar**: Pressione e segure em qualquer figurinha para ver um zoom animado antes de exportar.


<details>
<summary>
Instalação rápida (APK)
</summary>
<br>

1. Vá até a aba [Releases](https://github.com/Oyukihiro/StickerTLWS/releases).
2. Baixe o arquivo `app-release.apk` mais recente.
3. Instale no seu Android (permita a instalação de fontes desconhecidas se necessário).
4. Abra o app, coloque seu número e comece a exportar!

### Observações importantes:

* **Privacidade**: O StickerTLWS utiliza a biblioteca oficial do Telegram (TDLib). Suas credenciais são enviadas diretamente para os servidores do Telegram. O app não armazena suas mensagens ou contatos, apenas acessa seus pacotes de figurinhas.


* **Limites do WhatsApp**: O WhatsApp permite pacotes de no mínimo 3 e no máximo 30 figurinhas. O app gerencia esses limites para garantir que a exportação funcione sem erros.


* **Contribuições**: Sinta-se à vontade para abrir Pull Requests ou sugerir melhorias nas Issues. Toda ajuda é bem-vinda para tornar o app ainda melhor!

---

### Caso tenha algum problema, poste uma [issue](https://github.com/Oyukihiro/StickerTLWS/issues) detalhando o problema.


## Créditos e Tecnologias utilizadas:

* [TDLib](https://core.telegram.org/tdlib) - O motor por trás da integração com o Telegram.
* [FFmpeg Kit](https://github.com/arthenica/ffmpeg-kit) - Utilizado para a conversão de vídeos e animações.
* [Jetpack Compose](https://developer.android.com/compose) - UI moderna e declarativa.
* [Hilt](https://developer.android.com/training/dependency-injection/hilt-android) - Injeção de dependências.
* [Coil](https://coil-kt.github.io/coil/) - Carregamento eficiente de imagens e GIFs.
* [Lottie](https://github.com/airbnb/lottie-android) - Renderização de figurinhas TGS.
* [WebP Android](https://github.com/AureusApps/webp-android) - Encoder WebP para garantir compatibilidade com o WhatsApp.
