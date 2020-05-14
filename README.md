# cert-issuer

Este projeto tenta facilitar a emissão de certificados A1 da Soluti no Linux, e
também deve rodar em Windows e MacOS.

Quem sabe, com contribuições, podemos dar suporte a mais certificados e mais
provedores.


## Requerimentos

- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

O seu Linux deve ter uma forma prática de instalar ambos.


## Como usar

**IMPORTANTE**: Para salvar os certificados gerados pelo aplicativo, selecione o
diretório `/local/user`. Ele aponta para o diretório `user/` dentro deste
projeto. _Qualquer outro lugar será destruído ao fechar o aplicativo, e você
poderá **perder seus arquivos!**_

Mova esses arquivos para um local mais apropriado, e faça backup de documentos e
senhas criados durante o processo.

O seu diretório de usuário no sistema (e.g. `/home/usuario`) não está disponível
dentro do aplicativo por motivos de segurança.

### Soluti

```sh
./bin/run javaws src/soluti.jnlp
```

O aplicativo irá baixar algumas coisas e pedir autorização para outras.
Eventualmente, você deve ver a seguinte janela:

![soluti](https://i.imgur.com/2DOMyFt.png)

Siga os passos, de acordo com as instruções da Soluti.
