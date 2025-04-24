Estrutura inicial do portfólio de IA - Wallace

chatbot_eliza_clone.py

Uma versão simples do ELIZA usando NLTK

import nltk from nltk.chat.util import Chat, reflections

pairs = [ [r"(oi|ol[áa])", ["Olá, tudo bem? Como posso te ajudar?", "Oi! Em que posso te ajudar hoje?"]], [r"(qual seu nome??)", ["Meu nome é ELIZA Clone. Prazer!", "Sou apenas um bot humilde, sem nome bonito."]], [r"(adeus|tchau)", ["Tchau! Foi bom conversar com você.", "Até mais!"]], [r"(.*)", ["Por que você diz '%1'?"]] ]

chatbot = Chat(pairs, reflections)

if name == "main": print("Bem-vindo ao ELIZA Clone! (pressione Ctrl+C para sair)") chatbot.converse()

classificador_simples.py

Um modelo de machine learning simples que classifica o tipo de aplicação com base em palavras-chave

from sklearn.feature_extraction.text import CountVectorizer from sklearn.naive_bayes import MultinomialNB from sklearn.pipeline import make_pipeline

Base de dados simples

dados = [ "Diagnóstico de câncer por imagem", "Plataforma de ensino com aprendizado adaptativo", "Sistema automatizado de produção industrial", "Chatbot para atendimento ao cliente", "Análise preditiva para mercado financeiro" ]

categorias = [ "Saúde", "Educação", "Indústria", "Serviços", "Finanças" ]

modelo = make_pipeline(CountVectorizer(), MultinomialNB()) modelo.fit(dados, categorias)

Teste

amostra = ["Reconhecimento de imagem para diagnóstico médico"] print("Categoria prevista:", modelo.predict(amostra)[0])

Exemplo de README.md (resumo do projeto)

"""

Inteligência Artificial: Da Teoria ao Código

Este projeto é uma extensão prática do TCC de Wallace, explorando conceitos fundamentais da história da Inteligência Artificial e suas aplicações modernas.

Estrutura do Projeto

chatbot_eliza_clone.py: simulação de um chatbot estilo ELIZA

classificador_simples.py: modelo de ML que classifica tipos de aplicação por texto

documentacao_estrategica/: visão de gestão de TI com foco em IA


Visão Geral

Este repositório mescla Engenharia de Software com Gestão de Tecnologia da Informação, baseado no estudo sobre evolução da IA. """

Próximos arquivos a serem criados:

- visualizacao_dados.py (gráficos sobre evolução da IA)

- metodologia_IA_gestao.pdf (resumo da metodologia do TCC)

- roadmap_TI_IA.md (implementação de IA em empresas)

- desafios_eticos.md (visão crítica sobre riscos)



Tudo isso será incluído aos poucos ou posso gerar os arquivos conforme você for me pedindo.

print("Estrutura atualizada com classificador. Suba no GitHub com a pasta 'inteligencia-artificial-portifolio'")


