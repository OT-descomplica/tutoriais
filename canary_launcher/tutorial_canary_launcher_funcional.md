# Tutorial do Canary-Launcher Funcional

### O que é o Canary-Launcher:
É um programa para o sistema operacional Windows que:
- ✅ instala o cliente do otserv.
- ✅ checa se existe atualizações depois de instalado e, se houver, atualiza o cliente do usuário.
- ✅ quando o cliente estiver instalado e atualizado, ele abre o cliente direto pelo programa.
 
## Criando uma conta no GITHUB.COM e criando um FORK do repositório do código fonte do Canary-Launcher:
- Crie uma conta em https://github.com
- Crie um fork (garfo) do repositório do Canary-Launcher para o seu github em https://github.com/opentibiabr/canary-launcher/fork e edite o nome do repositório da forma que quiser.

## Baixando e editando o código fonte do Canary-Launcher:
O primeiro passo é baixar o código fonte do projeto do CANARY-LAUNCHER da OtservBR em seu repositório no github:
- :star: [canary-launcher](https://github.com/opentibiabr/canary-launcher/archive/refs/heads/main.zip)
- Depois abra o arquivo `src/MainWindow.xaml.cs` e encontre `"https://raw.githubusercontent.com/opentibiabr/canary-launcher/main/launcher_config.json"` e
substitua o `opentibiabr/canary-launcher` pelo nome do seu usuário no github/nome do repositório do seu launcher: por exemplo o meu `"https://raw.githubusercontent.com/holybaiak/tibiaclient13x/main/launcher_config.json"`.
- Em seguida, faça o mesmo procedimento da etapa acima em `src/SplashScreen.xaml.cs`.

## Compilando o programa em Windows com Visual Studio 2022 no modo 'Solution':
:interrobang: O que seria ese modo Solution? Seria um projeto (no caso o programa do launcher) contido dentro de uma solução. Apesar do nome, uma solução não é uma "resposta". Ela é apenas um contêiner de um ou mais projetos relacionados, juntamente com informações de build, configurações de janela do Visual Studio e arquivos diversos que não estão associados a nenhum projeto específico.

## Baixando e instalando o Visual Studio 2022:
O Visual Studio 2022 é o programa que iremos usar para compilar o código fonte do launcher, basta baixar no link: 
- :star: [Visual Studio 2022 Community](https://visualstudio.microsoft.com/pt-br/thank-you-downloading-visual-studio/?sku=Community&rel=17)
- Após o donwload, na tela inicial do Visual Studio, no produto Visual Studio Community 2022, clique no botão Instalar.
- Na próxima tela, em 'Cargas de trabalho', selecione 'Desenvolvimento de desktop com .NET'.
- Em seguida, em Pacotes de idiomas, selecione Inglês.

## Baixando e instalando o .NET 6.0:
Baixar no link: 
- :star: [.NET 6.0](https://dotnet.microsoft.com/en-us/download/dotnet/6.0)
- Basta clicar em instalar.

## Compilando o Canary-Launcher:
Open CanaryLauncherUpdate.csproj on Visual Studio 2022, select Release in the drop down menu then go to the menu Build > Build Solu