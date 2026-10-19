# Central Quarta Opinião — projeto Android inicial

Este projeto envolve o protótipo web em um aplicativo Android simples usando WebView.
Identidade visual: preto, azul neon e vermelho. O conteúdo do protótipo está em
`app/src/main/assets/index.html`.

## O que já está incluído
- Aplicativo Android com nome Central Quarta Opinião.
- Tela web do protótipo embutida no aplicativo.
- JavaScript habilitado e armazenamento local do navegador habilitado.
- Telas de Início, Roteiros, Agenda, Convidados e Comercial.
- Gerador demonstrativo de texto, edição e aprovação manual.

## O que ainda não está incluído
- Integração com IA real.
- Sincronização/backup em nuvem.
- Publicação automática nas redes sociais.
- Ícone gráfico definitivo e testes em diferentes aparelhos.
- APK pré-compilado.

## Como gerar o APK gratuitamente
1. Instale o Android Studio no computador.
2. Descompacte este projeto.
3. No Android Studio, escolha **Open** e selecione a pasta `CentralQuartaOpiniaoAndroid`.
4. Aguarde a sincronização do Gradle. Se solicitado, instale Android SDK Platform 35 e um JDK compatível com Android Studio.
5. Use **Build > Build APK(s)**.
6. O APK de depuração normalmente aparece em `app/build/outputs/apk/debug/app-debug.apk`.
7. Transfira o APK para seu Android e instale, autorizando a instalação de apps desta origem apenas se confiar no arquivo criado por você.

## Observações
Este é um ponto de partida para desenvolvimento, não uma versão testada/assinada para distribuição na Play Store.
O botão de copiar usa a API de clipboard do navegador; em algumas versões de WebView pode ser necessário adaptar a implementação.

## Compilar usando apenas o celular (GitHub Actions)
1. Crie uma conta em https://github.com se ainda não tiver.
2. No navegador do celular, crie um repositório novo e vazio chamado `CentralQuartaOpiniao`.
3. Use **Add file > Upload files** para enviar os arquivos/pastas deste projeto. Inclua também a pasta oculta `.github/workflows` e o arquivo `android-apk.yml`.
4. Faça o commit na branch `main`.
5. Abra a aba **Actions**, escolha **Gerar APK Android** e toque em **Run workflow** se não tiver iniciado automaticamente.
6. Quando terminar com sucesso, abra a execução concluída, role até **Artifacts** e baixe `Central-Quarta-Opiniao-APK`.
7. Extraia o ZIP baixado para obter `app-debug.apk` e abra no Android. Talvez seja necessário autorizar a instalação desta origem.

A compilação na nuvem é feita pelo GitHub Actions. O APK resultante é de depuração e não é assinado para publicação na Play Store. Não compartilhe credenciais nem tokens pessoais.
