## Pré-requisitos

### 1. Instalar o NodeJS versão 8 (https://nodejs.org/dist/latest-v8.x/)
  Observação: Verificar no terminal se o npm e o node estão instalados corretamente. Se necessário, adicionar pasta do zip ao PATH. Pode também baixar invez de fazer desta forma, baixar o instalador do node que é o arquivo com final .msi

### 2. Instalar o pacote windows-build-tools pelo npm (npm install --global windows-build-tools) 
  Observação: Este comando deve ser executado no "PowerShell" como admnistrador e não no "Terminal" . Talvez seja necessário executar esse comando múltiplas vezes, pois o programa pode travar durante a instalação do python e do visual studio build tools. Reiniciar o aparelho e tentar novamente caso isso ocorra.

### 3. Instalar o Ruby versão 2.3.3 (https://rubyinstaller.org/downloads/archives/)
* Observação: A versão do ruby precisa ser essa, pois o projeto da Tray utiliza uma versão antiga da linguagem.

* 3.1 - Ir nas "variaveis de ambiente" do computador, na parte do "PATH" , aperte em editar. Será listado todos os endereços que estão dentro da variável "PATH". Aperte em "novo" e adicione a pasta \bin para o PATH no final (ex.: D:\Programas\Ruby\ruby-2.3.3-x64-mingw32\bin)

* 3.2 - Verificar se o programa "gem" está instalado usando este comando "gem" no terminal(cmd). Caso retorne que o comando não é reconhecido, não existe ou algo do tempo, este erro é causado por conta do SSL. A configuração que deve ser feita é acessar no Windows o caminho "c: \ Usuários \ seu nome de usuário " e criar um arquivo com nome .gemrc pelo bloco de notas ou algo do tipo(lembrando que o arquivo tem que ter nome .gemrc e não pode ser por exemplo, .gemrc.txt .gemrc.zip se não vai dar erro, então ao criar pelo bloco de notas remova a extensão final .txt no nome do arquivo) e dentro dele você ira adicionar o seguinte comando: 

```
:ssl_verify_mode: 0
```


### 4. Instalar as seguintes bibliotecas no terminal:
  * gem install faraday -v 1.0.1
  * gem install launchy -v 2.4.3
  * gem install opencode_theme

  * Observação: Caso tenha algum problema durante essa fase de instalação do ruby/libs, verifique a thread do projeto: https://github.com/tray-tecnologia/opencode_theme/issues/44

### 5. Baixar o opencode workflow (https://github.com/tray-tecnologia/opencode-workflow), e seguir instalação conforme o README.md

### 6. As credenciais de acesso são individuais e devem ser geradas na plataforma.
* Obs.: Toda vez que publicar um tema ele não pode ser editável mais, então é preciso que faça novamente a etapa 5 tópico "Configuração/Uso" caso deseja editar um novo tema.

### 7. Pode meter bronca!
