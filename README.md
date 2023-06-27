# EPOS_PYTHON
Connecting Epos Step-Motor with python and create executable
Descrição
Interface para operação com envio de instruções de comando á Controladoras Maxon tipo EPOS, acopladas à um motor de giro. A interface permite comunicação direta com a controladora, podendo ativar funções sem a utilização de um software e maior flexibilidade para aplicações.

Instalação
Para usar o software você deve ter os seguintes pré-requisitos:
Python >=3.7.x
EPOS 0, 1, 2, 3, 4, P
Computador Sistema Operacional Linux ou Windows
Motor compatível com controladora
A Interface foi desenvolvida utilizando python. As seguintes bibliotecas foram utilizadas:

CustomTKInter
ctypes
Para comunicação do programa com a controladora, é necessário o arquivo .dll contendo a biblioteca dinâmica para instruir o programa a executar as funções pré programadas na controladora.

Após estabelecida a comunicação, executa-se o programa .py para controlar o motor.

Os parâmetros para conexão podem ser obtidos pelo gerenciamento de dispositivo ou pelo EPOS Studio.

Após preenchimento correto dos parâmetros, o usuário deve selecionar pode optar entre duas funções, ou a quantidade de steps ou definir um perfil de velocidades contínuo. Para isso, ele deve utilizar o 'slider' na parte inferior os parâmetros e clicar no botão "Enviar Comando Steps" para girar a quantidade escolhida ou "Enviar Comando Velocidade" Para girar na velocidade escolhida

Para Embarcar o programa, utilizou-se o PyInstaller (Pode-se ser obtido utilizado o comando 'pip install pyinstaller') e criou-se um executável do programa. Este executável funciona em OS Windows, porém o mesmo procedimento pode ser utilizado para gerar um executável para OS Linux ou Ubuntu. Assim, é possivel executar o programa sem a necessidade de um interpretador, no caso o python, e consequentemente, pode ser utilizado no sistema embarcado.

