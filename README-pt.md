Descrição
==================

Este pacote tem por objetivo armazenar cenas utilizadas no simulador CoppeliaSim Edu (https://coppeliarobotics.com/downloads) projetadas para trabalhar juntamente com o ROS (Robot Operating System) por meio do ROS Interface API (https://www.coppeliarobotics.com/helpFiles/en/rosInterf.htm). Deste modo, as cenas apresentadas neste pacote são capazes de ler e enviar informações ao ROS.  

 

 

Configuração do sistema utilizado 
-------------------------------

* Ubuntu 18.04.4 (http://releases.ubuntu.com/18.04.4/) 
* ROS Melodic (http://wiki.ros.org/melodic/Installation/Ubuntu) 

Instalando o CoppeliaSim Edu no ubuntu 18.04 
------------------------------------------------

* Baixe a versão desejada no endereço https://coppeliarobotics.com/ubuntuVersions 
  - Para a versão "CoppeliaSim_Edu_V4_0_0_Ubuntu18_04" siga os paços a seguir: 

```
$ cd ~/ 
$ wget https://coppeliarobotics.com/files/CoppeliaSim_Edu_V4_0_0_Ubuntu18_04.tar.xz 
```

* Extraia o arquivo 

```
$ tar -xf CoppeliaSim_Edu_V4_0_0_Ubuntu18_04.tar.xz 
```

* É preciso adicionar a biblioteca do ROSInterface na pasta principal do compiledRosPlugins. A biblioteca já encontrasse compilada dentro da pasta "compiledRosPlugins". Vamos copiar o arquivo “libsimExtROSInterface.so” para a página principal.

```
$ cd ~/CoppeliaSim_Edu_V4_0_0_Ubuntu18_04/
$ cp compiledRosPlugins/libsimExtROSInterface.so libsimExtROSInterface.so
```

Executando 
-------------------------------------

* Para executar o CoppeliaSim, basta executar o arquivo “coppeliaSim.sh”. É preciso estar com o **roscore** inicializado. 

```
$ roscore
$ cd ~/CoppeliaSim_Edu_V4_0_0_Ubuntu18_04/
$ ./coppeliaSim.sh
```

* Verifique no terminal se a seguinte mensagem aparece 
  - Plugin 'ROSInterface': load succeeded. 


* O coppeliaSim deve abrir, é possível criar um atalho para facilitar a inicialização. Agora é possível executar qualquer uma das cenas presentes neste repositório.







