# MineMod

Mod para o Minecraft Java **26.3**, com Fabric. Aqui ficam só as versões prontas para baixar.

## Instalar ou atualizar (Windows)

1. Se você nunca abriu o Minecraft Java neste computador, abra o Minecraft Launcher uma vez e entre com sua conta.
2. Baixe o **[MineMod-Instalador.exe](https://github.com/josecldjr/minemod-releases/releases/latest/download/MineMod-Instalador.exe)**.
   Se o navegador disser que o arquivo "não é baixado com frequência", escolha **Manter**.
3. Dê dois cliques no arquivo. Se aparecer **"O Windows protegeu o computador"**, clique em **Mais informações** e
   depois em **Executar assim mesmo**. O aviso aparece porque o instalador não tem assinatura digital.
4. Clique em **Instalar**. No fim, clique em **Abrir o Minecraft**, escolha o perfil **MineMod** e clique em **Jogar**.

Para atualizar, abra o mesmo instalador de novo. Ele confere se há versão nova e instala sozinho.

O instalador cria um perfil próprio, **MineMod**, com pasta separada (`%APPDATA%\.minecraft\minemod`). Na primeira
vez ele copia suas opções e sua lista de servidores. Seus outros perfis, mundos e mods não são mexidos. Ele instala
o Fabric Loader, a Fabric API, o MineMod e alguns mods de outros autores, baixados direto do
[Modrinth](https://modrinth.com):

| Para quê | Mods |
|---|---|
| Deixar o jogo mais leve | [Sodium](https://modrinth.com/mod/sodium), [ImmediatelyFast](https://modrinth.com/mod/immediatelyfast), [FerriteCore](https://modrinth.com/mod/ferrite-core), [Entity Culling](https://modrinth.com/mod/entityculling) |
| Jogar melhor | [Xaero's Minimap](https://modrinth.com/mod/xaeros-minimap), [Inventory Profiles Next](https://modrinth.com/mod/inventory-profiles-next) (com [libIPN](https://modrinth.com/mod/libipn) e [Fabric Language Kotlin](https://modrinth.com/mod/fabric-language-kotlin)), [JEI](https://modrinth.com/mod/jei) (com [MezzConfig](https://modrinth.com/mod/mezzconfig)) |

Outros mods que você puser na pasta `%APPDATA%\.minecraft\minemod\mods` ficam lá quando o instalador atualiza.

## Se o Windows bloquear sem a opção "Executar assim mesmo"

Isso acontece quando o **Controle Inteligente de Aplicativos** do Windows 11 está ligado. Nesse caso, instale à mão:

1. Instale o **Fabric Loader 0.20.1** para o **Minecraft 26.3** com o [instalador oficial do Fabric](https://fabricmc.net/use/installer/).
2. Na [versão mais recente](https://github.com/josecldjr/minemod-releases/releases/latest), baixe os dois arquivos `.jar`
   (`minemod-….jar` e `fabric-api-….jar`) e coloque na pasta `%APPDATA%\.minecraft\mods`.
3. Se quiser, baixe também os mods da tabela acima, nas páginas deles no Modrinth (versão para Fabric e Minecraft 26.3),
   e coloque na mesma pasta. Para entrar no servidor, só o MineMod e a Fabric API são obrigatórios.
4. No Minecraft Launcher, escolha o perfil do Fabric e clique em **Jogar**.

## O que vem em cada versão

| Arquivo | O que é |
|---|---|
| `MineMod-Instalador.exe` | instalador e atualizador |
| `minemod-X.jar` | o mod |
| `fabric-api-X.jar` | biblioteca que o mod exige, baixada do [maven oficial do Fabric](https://maven.fabricmc.net/) |
| `manifest.json` | lista que o instalador lê, com o SHA-256 de cada arquivo (os mods de outros autores aparecem nela com o endereço do Modrinth) |
