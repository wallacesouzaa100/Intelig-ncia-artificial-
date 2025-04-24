

Arquivo: chatbot_eliza_clone.py
import nltk
from nltk.chat.util import Chat, reflections

pairs = [
    [r"(oi|ol[áa])", ["Olá, tudo bem? Como posso te ajudar?", "Oi! Em que posso te ajudar hoje?"]],
    [r"(qual seu nome\??)", ["Meu nome é ELIZA Clone. Prazer!", "Sou apenas um bot humilde, sem nome bonito."]],
    [r"(adeus|tchau)", ["Tchau! Foi bom conversar com você.", "Até mais!"]],
    [r"(.*)", ["Por que você diz '%1'?"]]
]

chatbot = Chat(pairs, reflections)

if __name__ == "__main__":
    print("Bem-vindo ao ELIZA Clone! (pressione Ctrl+C para sair)")
    chatbot.converse()



Arquivo: classificador_simples.py

from sklearn.feature_extraction.text import CountVectorizer
from sklearn.naive_bayes import MultinomialNB
from sklearn.pipeline import make_pipeline

dados = [
    "Diagnóstico de câncer por imagem",
    "Plataforma de ensino com aprendizado adaptativo",
    "Sistema automatizado de produção industrial",
    "Chatbot para atendimento ao cliente",
    "Análise preditiva para mercado financeiro"
]

categorias = ["Saúde", "Educação", "Indústria", "Serviços", "Finanças"]

modelo = make_pipeline(CountVectorizer(), MultinomialNB())
modelo.fit(dados, categorias)

amostra = ["Reconhecimento de imagem para diagnóstico médico"]
print("Categoria prevista:", modelo.predict(amostra)[0])




3. Visão Estratégica de Gestão de TI (em construção)

Metodologia estruturada baseada no TCC (definição do problema, coleta de dados, modelo, monitoramento)

Roadmap de implementação de IA em ambientes corporativos

Discussões sobre ética, viés algorítmico, privacidade e impactos sociais


Arquivos planejados:

documentacao_estrategica/metodologia_IA_gestao.pdf

roadmap_TI_IA.md

desafios_eticos.md



---

Sobre o Autor

Wallace Antunes Souza é Engenheiro de Software em formação, com MBA em Gestão de Tecnologia da Informação. Apaixonado por IA e transformação digital, busca aplicar tecnologia com propósito e impacto real.

> "A IA não é só tecnologia, é decisão estratégica."






Licença: MIT

Contato: linkedin.com/in/seu-perfil 


