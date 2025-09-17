[Read in english](README.md)

# 🤖 economIA: Seu Guru Pessoal de Economia

Cansado de procurar em anotações infinitas e desorganizadas antes de uma prova? Frustrado com respostas genéricas de IAs que claramente nunca sofreram em uma aula de Macroeconomia?

**Não tema!** Apresento a **economIA**, uma agente de IA que foi alimentada à força com as minhas anotações da faculdade. Esta não é uma IA qualquer; é uma IA com graduação em andamento, especialista em sobreviver a Economia 101.

## O Problema: Caos de Dados vs. A Prova Final

Sejamos realistas, nossas anotações são uma bagunça. Elas são um tesouro caótico de informações vitais, insights rabiscados e súplicas desesperadas aos deuses da economia. Isso são "dados não estruturados", e são ouro puro, mas tentar encontrar um conceito específico neles é como tentar achar um único estudante não deprimido na semana de provas.

## A Solução: Uma IA Que Lê as Anotações Por Você!

A agente **economIA** resolve este problema de forma brilhante. Usando uma técnica chamada RAG (Geração Aumentada por Recuperação), ela transforma aquela pilha caótica de arquivos `.txt` em uma base de conhecimento pesquisável e inteligente.

**Como ela te ajuda a estudar:**
* **Respostas Precisas**: Faça uma pergunta específica como "Qual era a do Mercantilismo?" e receba uma resposta baseada *apenas* no que o professor ensinou (e no que eu consegui anotar). Chega de fatos estranhos e aleatórios da internet!
* **Conexão de Conceitos**: Você pode pedir para ela conectar ideias entre diferentes matérias. "Crie um debate entre Adam Smith e Karl Marx" se torna uma tarefa trivial, não uma sessão de 3 horas na biblioteca.
* **Revisão Instantânea**: É o parceiro de estudos definitivo. Nunca se cansa, nunca tenta mudar de assunto para o jogo de ontem à noite e está disponível 24/7.

## As Entranhas e a Glória Técnica

* **O Cérebro (LLM)**: Movido pelo Llama 3, rápido como um raio, via Groq. Pensa mais rápido do que você consegue dizer "oferta e demanda".
* **A Memória (Vector Store)**: Usa o FAISS para criar um banco de dados vetorial de alta velocidade e pesquisável com as minhas anotações. É como uma memória fotográfica, mas para economia.
* **A Bibliotecária (LangChain)**: O framework que orquestra todo o processo, garantindo que as anotações certas sejam recuperadas para responder às suas perguntas.

## Como Ligar a Agente

1.  **Clone o Repositório**: Obtenha todos os arquivos em sua máquina.
2.  **Faça o Upload para o Colab**: Abra o notebook `AgenteIAEconomia.ipynb` no Google Colab.
3.  **Alimente a Máquina**: Certifique-se de fazer o upload dos arquivos `.txt` com as anotações (`Economia Política.txt`, `História econômica geral.txt`, `Macroeconomia.txt`) para o diretório `/content/` em sua sessão do Colab.
4.  **Entregue as Chaves**: Você precisará de uma chave de API gratuita da [Groq](https://groq.com/). Salve essa chave nos "Secrets" do seu Colab com o nome `GROQ_API_KEY`.
5.  **Execute Todas as Células**: Sente-se, execute o notebook e veja a mágica acontecer.
6.  **Pergunte à Vontade!**: Vá para a última célula e digite suas perguntas mais mirabolantes de economia na variável `pergunta`.

### Exemplo de Sessão

```python
# O que você faz:
pergunta = "crie uma briga entre karl marx e adam smith"

# O que a IA faz (baseado nas minhas anotações!):
--- Pergunta ---
crie uma briga entre karl marx e adam smith

--- Resposta Gerada ---
Karl Marx: "Senhor Smith, sua 'mão invisível' é apenas uma batedora de carteiras para a burguesia, roubando a mais-valia criada pelo proletariado!"

Adam Smith: "Meu caro Marx, você vê exploração em todo lugar! Minha 'mão invisível' é a harmonia do autointeresse criando o bem social. Seu sistema cria uma miséria igual para todos, exceto para aqueles encarregados da 'igualdade'."
```
