Projeto baseados em Vagrant. Neste exemplo, estou desenvolvendo a infra-estrutura como código e subindo uma distro do Ubuntu com as sequintes especificações:
    Nome da maquina: projeto-vagrant
    Memoria ram: 1024
    pasta compartilhada: config.vm.synced_folder "./vagrant", "/var/www/html"
    tipo de placa de rede: bridged
    Roteamento de porta: da porta 80 a 8080
    Atualização e instalação de pacotes nginx com provision