# capitaoPlaneta

Projeto que visa usar as boas práticas de desenvolimento para criar uma aplicação de adoação, de pets <<NOME DO PROJETO>>

## Aprendizados buscados

- TDD
- Arquitetura limpa
- DDD
- EDD

## MVP

Plataforma de cadastro de usuários e pets, com mural de fotos e recados que possibilite a interação entre os envolvidos no processo.

### Requisitos

- transparencia
- segurança
- estabilidade

### Funcionalidades

- Registrar um usuario, cuidador/doador.
- Cadastrar um pet ?
-- abrir processo de adoção.
- apadrinhamento ?
-- criar Lista de compras

## Cenários
- Jornada do usuario

Quero me cadastrar na plataforma.
Quero poder adotar um pet.
Dado que estou cadastrado quero ter um mural com os pets que ajudei/adotei. (engajamento)

- Jornada do pet

Quero cadastrar um pet na plataforma.
Dado que eu cadastrei um pet eu quero criar uma história para ele.
Dado que eu cadastrei um pet quero ajuda para cuidar dele antes de entrega-lo.
Dado que eu cadastrei um pet quero disponibiliza-lo para adoção.

## Entidades

### Pet

- dados pessoais
- historia : registro ( guarda, pré guarda, tratamento, passeio)

SerAdotado:
  - Processo de adoção precisa de acompanhamento, etapas.
  -- verificar o lar, verificar o candidato, dar relatos pós adoção.
  
SerCadastrado:
Tratamentos(vacina, castração, veterinario)
EditarSuaHistoria.
  - Apenas o guardião pode editar o nome do pet.
  - midia sensivel precisa de analise para ser postada (nao sei como)

### PetLover
tipo :  filantropo, guardiao_fixo, guardiao_temporario

- dados pessoais
- historia : registro ( guarda, doação, visita, passeio, tratamento)
 adotarUmPet
 EditarSuaHistoria.

### História
 - histórico : pet+ , petlover+.
 - CriarHistoria
 - EditarHistoria

## contexto

Delimitar as intenções das entidades com base no contexto que ela pertence.

- Guarda fixa : situação que o pet foi adotado.
- Guarda compartilhada : situação que o pet foi adotado e precisa de ajuda.
- Guarda temporária : situação que o pet tem um lar temporário e precisa de um dono.