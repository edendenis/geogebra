# Como configurar/instalar/usar o `GeoGebra` no `Linux Ubuntu`

## Resumo

Neste documento estão contidos os principais comandos e configurações para configurar/instalar/usar o `GeoGebra` no `Linux Ubuntu`.

## _Abstract_

_This document contains the main commands and settings for configuring/installing/use `GeoGebra` on `Linux Ubuntu`._

## Descrição [2]

### `GeoGebra`

O `GeoGebra` é uma poderosa plataforma de matemática interativa de código aberto, projetada para auxiliar professores e alunos na exploração e compreensão de conceitos matemáticos. Combina recursos de geometria, álgebra, planilha e cálculo em uma única interface amigável, permitindo a criação de construções matemáticas dinâmicas e a visualização de gráficos em tempo real. O `GeoGebra` é amplamente utilizado em salas de aula em todo o mundo, pois oferece uma abordagem prática e visual para o ensino e a aprendizagem da matemática, além de ser uma ferramenta valiosa para explorar conceitos matemáticos de forma intuitiva e interativa. Com suas capacidades de manipulação e representação de objetos matemáticos, o `GeoGebra` é uma escolha preferida para o ensino e a exploração da matemática, desde o nível básico até o avançado.


## 1. Instalar o `GeoGebra` no `Linux Ubuntu` [1]

Para instalar o `GeoGebra` no `Linux Ubuntu`, você pode seguir estas etapas:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Alt + T`


2. Certifique-se de que seu sistema esteja limpo e atualizado.

    2.1 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.2 Remover pacotes `.deb` antigos ou duplicados do cache local. É útil para liberar espaço, pois remove apenas os pacotes que não podem mais ser baixados (ou seja, versões antigas de pacotes que foram atualizados). Digite o seguinte comando: `sudo apt autoclean`

    2.3 Remover pacotes que foram automaticamente instalados para satisfazer as dependências de outros pacotes e que não são mais necessários. Digite o seguinte comando: `sudo apt autoremove -y`

    2.4 Buscar as atualizações disponíveis para os pacotes que estão instalados em seu sistema. Digite o seguinte comando e pressione `Enter`: `sudo apt update`

    2.5 **Corrigir pacotes quebrados**: Isso atualizará a lista de pacotes disponíveis e tentará corrigir pacotes quebrados ou com dependências ausentes: `sudo apt --fix-broken install`

    2.6 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.7 Para ver a lista de pacotes a serem atualizados, digite o seguinte comando e pressione `Enter`:  `sudo apt list --upgradable`

    2.8 Realmente atualizar os pacotes instalados para as suas versões mais recentes, com base na última vez que você executou `sudo apt update`. Digite o seguinte comando e pressione `Enter`: `sudo apt full-upgrade -y`
    


4. Em seguida, você pode instalar o GeoGebra usando o comando apt. Execute o seguinte comando: `sudo apt install geogebra -y`

    - O sistema irá solicitar sua senha de administrador. Digite-a e pressione Enter.

5. O Ubuntu irá mostrar uma lista de pacotes a serem instalados e a quantidade de espaço em disco que eles ocuparão. Confirme a instalação digitando `Y` e pressionando `Enter`.

    - Aguarde enquanto o sistema baixa e instala o GeoGebra e suas dependências.

6. Uma vez concluída a instalação, você pode iniciar o GeoGebra a partir do menu de aplicativos do Ubuntu ou digitandono terminal: `geogebra`

Agora você deve ter o GeoGebra instalado e pronto para uso no seu sistema Ubuntu.



```python
### 1.1 Codigo completo para configurar/instalar

Para instalar o `GeoGebra` no Linux Ubuntu sem precisar digitar linha por linha, você pode seguir estas etapas:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Alt + T`

2. Digite o seguinte comando e pressione `Enter`:

    ```
    sudo apt clean                                                            
    sudo apt autoclean
    sudo apt autoremove -y
    sudo apt update
    sudo apt --fix-broken install
    sudo apt clean
    sudo apt list --upgradable
    sudo apt full-upgrade -y
    sudo apt install geogebra -y
    geogebra
    ```

```

## Referências

[1] OPENAI. ***Instalação do geogebra no linux.*** Disponível em: <https://chat.openai.com/c/49c2d80f-fb06-4cb0-a8aa-cfbc103bc797> (texto adaptado). ChatGPT. Acessado em: 29/09/2023 23:13.

[2] OPENAI. ***Vs code: editor popular:*** Disponível em: <https://chat.openai.com/c/b640a25d-f8e3-4922-8a3b-ed74a2657e42> (texto adaptado). ChatGPT. Acessado em: 23/11/2023 15:53.

