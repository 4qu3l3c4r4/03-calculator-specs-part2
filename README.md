# Calculator-Specs-Screen Objects
Basic structure Appium android project

### Instalando Ambiente no Mac

```ruby
a. Instalar o Homebrew:
   /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"r
   
b. Instalar JDK para o Mac:
   http://www.oracle.com/technetwork/java/javase/downloads/index.html

c. Instalando e configurando o rbenv:
   brew install rbenv
   echo 'eval "$(rbenv init -)"' >> ~/.bash_profile
   rbenv install -l
   rbenv install 2.4.0 #Ou versão superior estável
   rbenv local 2.4.0

d. Instalar Android Studio
   https://developer.android.com/studio/index.html?hl=pt-br
   
e. Instalar Appium Desktop
   http://appium.io/ => Clique em download e baixe a versão mais recente para o seu SO
```

### Variáveis de Ambiente JAVA
```ruby
Abrir arquivo de configuração
open ~/.bash_profile

Preencher com:
export JAVA_HOME=$(/usr/libexec/java_home)
export PATH=$JAVA_HOME/bin:$PATH 
```

### Variáveis de Ambiente do Android

```ruby
Abrir arquivo de configuração
open ~/.bash_profile

Preencher com:
export ANDROID_HOME=/Users/<usuario>/Library/Android/sdk
export PATH=$ANDROID_HOME/tools/bin:$PATH
export PATH=$ANDROID_HOME/tools:$PATH
export PATH=$ANDROID_HOME/platform-tools:$PATH
export PATH=$ANDROID_HOME/platform-tools/adb:$PATH
export PATH=$ANDROID_HOME/emulator/:$PATH

NOTE: Trocar o <usuario> pelo nome do seu usuário
```

### Instalando Gerenciador de gems do Ruby

```ruby
gem install bundler
```

### Executando o Projeto :dart:

```ruby
1. Faça um clone do projeto:
   git clone https://github.com/4qu3l3c4r4/calculator-specs.git

2. Acesse a pasta pelo terminal e execute o comando:
   bundle

3. Emulando android virtual device: 
   emulator @"<Nome do seu emulator>"&
   
4. Abra o Appium e inicie o servidor do mesmo.

5. Executando os cenários da feature "Multiplicar": 
   cucumber
```
