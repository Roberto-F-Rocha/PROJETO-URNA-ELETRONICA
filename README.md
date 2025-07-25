# Urna Eletrônica Simplificada em C

Este projeto simula uma urna eletrônica básica para eleições estudantis, desenvolvida em linguagem C. O programa permite a definição do número de votantes, a realização de votações para Representante Estudantil e Presidente do Grêmio, e a contabilização dos votos.

## Funcionalidades

- **Definição de Votantes**: Permite configurar a quantidade mínima de discentes para a votação (mínimo de 31).
- **Votação**: Os usuários podem votar em candidatos para Representante Estudantil e Presidente do Grêmio. Os votos são registrados por números específicos para cada candidato.
- **Voto em Branco/Nulo**: Opções para votar em branco ou anular o voto.
- **Contabilização de Votos**: Exibe os resultados da votação para ambos os cargos, incluindo votos brancos e nulos.
- **Santinhos**: Permite visualizar os "santinhos" (informações dos candidatos) antes da votação.
- **Interface de Usuário**: Interface baseada em texto com menus para navegação.

## Como Compilar e Executar

### Pré-requisitos

- Um compilador C (como GCC).

### Compilação

Para compilar o programa, utilize o seguinte comando no terminal:

```bash
gcc urna__s2ok.c -o urna
```

### Execução

Após a compilação, execute o programa com:

```bash
./urna
```

## Detalhes do Código

O código utiliza funções para organizar as diferentes telas e funcionalidades da urna. As principais seções incluem:

- `main()`: Função principal que gerencia o fluxo do programa, o menu de opções e a lógica de votação.
- `tela_1()` e `tela_2()`: Funções para exibir as interfaces de votação para Representante e Presidente, respectivamente.
- Funções de Candidatos (`david()`, `vini()`, `polly()`, `karla()`, `dyego()`, `had()`, `lav()`): Exibem informações detalhadas de cada candidato.
- `erro()`: Exibe uma mensagem de erro genérica.
- `fim()`: Exibe uma mensagem de finalização.

**Observação**: O código inclui `windows.h` e `system("color 1F")`, o que indica que foi desenvolvido com foco em ambientes Windows. No entanto, o uso de `system("clear || cls")` tenta oferecer alguma compatibilidade com sistemas baseados em Unix/Linux para limpar a tela. Para uma experiência ideal, a execução em Windows é recomendada ou a adaptação das chamadas `system()` para o seu sistema operacional.

# Música do Mario

Uma característica interessante deste projeto é a inclusão da música tema do Mario, reproduzida através da função mario(). Esta função utiliza chamadas Beep() para gerar os sons e Sleep() para controlar as pausas entre as notas, simulando a melodia. A implementação envolveu um desafio significativo na identificação das frequências exatas para cada nota musical, a fim de reproduzir fielmente o tom original da música. Além disso, o ajuste preciso dos tempos de Sleep() foi crucial para garantir o ritmo e a cadência corretos da melodia, tornando a tarefa de programação ainda mais complexa e detalhada.

## Autores

- Roberto Fernandes Rocha
- Vinicius Anacleto de Almeida

Disciplina: Laboratório de Algoritmos
Professor: Dyego Magno
Universidade Federal Rural do Semi-Árido (UFERSA)


```
            - SANTINHOS -
----------                 ----------
|  /()\  |                 |   ()   |
|  (||)  |                 |  (||)  |
|   /\   |                 |   /\   |
|  /  \  |                 |  /  \  |
----------                 ----------

```


